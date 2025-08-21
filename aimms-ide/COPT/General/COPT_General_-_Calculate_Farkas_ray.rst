.. _option-COPT-calculate_farkas_ray:


Calculate Farkas Ray
====================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	No	



This option specifies whether COPT should compute the dual Farkas or primal ray when the LP is infeasible or unbounded. Possible values of this option are:



*	No
*	Yes




If this option is activated then COPT calculates a Farkas infeasibility proof once COPT detects that the model is infeasible. The Farkas infeasibility proof provides a dual unbounded vector. Adding this vector into any feasible solution to the dual model yields a new solution that is also feasible but improves the dual objective. This vector is passed to AIMMS instead of the normal level values for the constraints. Note that the general solvers option **Always Store Constraint Levels**  should be switched on.





If this option is activated then COPT calculates an unbounded ray once COPT detects that the model is unbounded. The unbounded ray is passed to AIMMS instead of the normal level values for the variables.





**Note** 

*	The Farkas infeasibility proof and the unbounded ray are only available for LP and RMIP models.
*	If the presolver detects infeasibility (or indicates that the model is InfeasibleOrUnbounded) then the Farkas infeasibility proof is not available. In that case, turn **Presolve**  off and reoptimize to obtain the Farkas infeasibility proof.
*	If the presolver detects unboundedness (or indicates that the model is InfeasibleOrUnbounded) then the unbounded ray is not available. In that case, turn **Presolve**  off and reoptimize to obtain an unbounded ray.
*	If you are using the barrier optimizer without crossover (see the options **LP Method**  and **Crossover** ) then the Farkas infeasibility proof and the unbounded ray are not available. 




**Learn more about** 

*	:ref:`option-AIMMS-always_store_constraint_levels`  
*	:ref:`option-COPT-crossover`  
*	:ref:`option-COPT-lp_method`  
*	:ref:`option-COPT-presolve`  
