

.. _option-AIMMS-cutoff:


Cutoff
======



:Type:	Floating point number	
:Range:	(-inf,inf)	
:Default:	Na	



Mixed Integer Problems in AIMMS are solved by branch and bound algorithms, in which a sequence of LP subproblems
is solved. These subproblems can be viewed as nodes in a tree; the root node being the LP relaxation of the
original MIP. Normally, the solution to the relaxation contains fractional-valued variables that should be
integer-valued according to the MIP definition. One of those variables is chosen for branching, and two new
subproblems are generated, each with more restrictive bounds for the branching variable. For example, for
binary variables, one subproblem fixes the variable at zero, and one subproblem fixes the variable at one.
If the solution of a subproblem contains again fractional values for the integer variables, then the process
is repeated. 

The generation of these subproblems is influenced by the option Cutoff in the following way. If the objective
function is to be minimized, then the nodes corresponding to subproblems, of which the objective value is larger
than Cutoff, then the node is considered as not promising enough and the node is "cut off" the tree. For MIPs
where the objective function is to be maximized, the opposite action takes place: the node is cut off the tree
if the objective function of the corresponding subproblem is smaller than Cutoff. The default value refers to
-inf for minimizing problems, and inf for maximizing problems.


**Note** 

*	The behavior of :ref:`SolverGurobi` differs slightly from :ref:`SolverCPLEX`. Assume we are minimizing and the cutoff value is 300. For CPLEX any solution with an objective value > 300 will not be acceptable, while for GUROBI any solution with an objective value >= 300 (including 300 itself) will not be acceptable. Therefore, if the objective value of 300 should also be acceptable for Gurobi then the cutoff value should be set to 300 + eps.
*	This option is also valid for MIQP and MIQCP problems.



