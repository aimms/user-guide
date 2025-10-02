.. _CPLEX_User_Cuts_and_Lazy_Constraints:


User Cuts and Lazy Constraints
==============================

In contrast to the cuts that CPLEX may automatically add while solving a problem, user cuts are those cuts that a user defines based
on information already implied about the problem by the constraints; user cuts may not be strictly necessary to the problem, but they
tighten the model. Lazy constraints are constraints that the user knows are unlikely to be violated, and in consequence, the user wants
them applied lazily, that is, only as necessary or not before needed. User cuts can be grouped together in a pool of user cuts. Likewise,
lazy constraints can also be grouped into a pool of lazy constraints.


**Pools** 

Sometimes, for a MIP formulation, a user may already know a large set of helpful cutting planes (user cuts), or can identify a group of
constraints that are unlikely to be violated (lazy constraints). Simply including these cuts or constraints in the original formulation
could make the LP subproblem of a MIP optimization very large or too expensive to solve. Instead, these situations can be handled by setting
up cut pools or pools of lazy constraints before MIP optimization begins.


In AIMMS, a constraint is added to the cut pool if the constraint has property 'IncludeInCutPool'. A constraint is added to the pool of
lazy constraints if the constraint has property 'IncludeInLazyConstraintPool'.


The principle in common between these two pools allows the optimization algorithm to perform its computations on a smaller model than it
otherwise might, in the hope of delivering faster run times. In either case (whether in the case of pools of user cuts or pools of lazy
constraints), the model starts out small, and then potentially grows as members of the pools are added to the model. Both kinds of pool
may be used together in solving a MIP model, although that would be an unusual circumstance. 


**Difference between user cuts and lazy constraints** 

However, there is an important distinction between these two concepts. 


Cuts may resemble ordinary constraints, but are conventionally defined to mean those which can change the feasible space of the continuous
relaxation but do not rule out any feasible integer solution that the rest of the model permits. A collection of cuts, therefore, involves
an element of freedom: whether or not to apply them, individually or collectively, during the optimization of a MIP model; the formulation
of the model remains correct whether or not the cuts are included. This degree of freedom means that if valid and necessary constraints are
mis-identified by the user and passed to CPLEX as user cuts, unpredictable and possibly incorrect results could occur. 


By contrast, lazy constraints represent simply one portion of the constraint set, and the model would be incomplete (and possibly would
deliver incorrect answers) in their absence. CPLEX always makes sure that lazy constraints are satisfied before producing any solution to
a MIP model. Needed lazy constraints are also kept in effect after the MIP optimization terminates, for example, when you change the problem
type to fixed-integer and re-optimize with a continuous optimizer. 


Another important difference between pools of user cuts and pools of lazy constraints lies in the timing by which these pools are applied.
CPLEX may check user cuts for violation and apply them at any stage of the optimization. Conversely, it does not guarantee to check them at
the time an integer-feasible solution candidate has been identified. Lazy constraints are only (and always) checked when an integer-feasible
solution candidate has been identified, and of course, any of these constraints that turn out to be violated will then be applied to the full
model. 


Another way of comparing these two types of pool is to note that the user designates constraints as lazy in the strong hope and expectation
that they will not need to be applied, thus saving computation time by their absence from the working problem. In practice, it is relatively
costly (for a variety of reasons) to apply a lazy constraint after a violation is identified, and so the user should err on the side of caution
when deciding whether a constraint should be marked as lazy. In contrast, user cuts may be more liberally added to a model because CPLEX is not
obligated to use any of them and can apply its own rules to govern their efficient use.


**Adding user cuts or lazy constraints through a callback** 

Instead of using a pool of user cuts, it is also possible to add cuts through a callback. This callback can be installed by calling the AIMMS
routine :any:`GMP::Instance::SetCallbackAddCut`. Adding user cuts through a callback gives more flexibility but can be more inefficient than
using a pool of user cuts.


A callback for lazy constraints can be installed by calling the AIMMS routine :any:`GMP::Instance::SetCallbackAddLazyConstraint`.


**Note** 

*	If the model uses lazy constraints (either through a callback or a pool) then CPLEX turns off dual reductions during preprocessing. (See the option **Preprocessing Reduction Types**.)
*	Indicator constraints cannot be used as user cut or lazy constraint.


**Learn more about** 

*	:any:`GMP::Instance::SetCallbackAddCut`
*	:any:`GMP::Instance::SetCallbackAddLazyConstraint`
*	:ref:`CPLEX_Indicator_Constraints` 
*	:ref:`option-CPLEX-preprocessing_reduction_types`  
