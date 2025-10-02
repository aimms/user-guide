.. _GUROBI_User_Cuts_and_Lazy_Constraints:


User Cuts and Lazy Constraints
==============================

Gurobi supports both user cuts and lazy constraints through callbacks. User cuts eliminate fractional solutions from LP relaxations.
Lazy constraints are constraints that are added to cutoff solutions that are integer feasible but undesirable. User cuts can be grouped
together in a pool of user cuts. Likewise, lazy constraints can also be grouped into a pool of lazy constraints.


**Adding user cuts or lazy constraints through a callback** 

A callback for user cuts can be installed by calling the AIMMS procedure :any:`GMP::Instance::SetCallbackAddCut`. A callback for lazy constraints
can be installed by calling the AIMMS procedure :any:`GMP::Instance::SetCallbackAddLazyConstraint`.


**Pools** 

Sometimes, for a MIP formulation, a user may already know a large set of helpful cutting planes (user cuts), or can identify a group of constraints
that are unlikely to be violated (lazy constraints). Simply including these cuts or constraints in the original formulation could make the LP
subproblem of a MIP optimization very large or too expensive to solve. Instead, these situations can be handled by setting up cut pools or pools
of lazy constraints before MIP optimization begins.


In AIMMS, a constraint is added to the cut pool if the constraint has property 'IncludeInCutPool'. A constraint is added to the pool of lazy
constraints if the constraint has property 'IncludeInLazyConstraintPool'.


The principle in common between these two pools allows the optimization algorithm to perform its computations on a smaller model than it
otherwise might, in the hope of delivering faster run times. In either case (whether in the case of pools of user cuts or pools of lazy
constraints), the model starts out small, and then potentially grows as members of the pools are added to the model. Both kinds of pool
may be used together in solving a MIP model, although that would be an unusual circumstance.


**Note** 

*	The option **Lazy Constraint Mode** determines how lazy constraints are handled by Gurobi.
*	If the model uses lazy constraints (either through a callback or a pool) then Gurobi turns off dual reductions during preprocessing. (See the option **Dual Reductions**.)
*	Indicator constraints cannot be used as user cut or lazy constraint.


**Learn more about** 

*	:ref:`option-GUROBI-dual_reductions` 
*	:ref:`GUROBI_Indicator_Constraints` 
*	:ref:`option-GUROBI-lazy_constraint_mode`  
*	:any:`GMP::Instance::SetCallbackAddCut`
*	:any:`GMP::Instance::SetCallbackAddLazyConstraint`
