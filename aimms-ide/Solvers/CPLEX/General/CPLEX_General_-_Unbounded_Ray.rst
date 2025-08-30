.. _option-CPLEX-unbounded_ray:


Unbounded Ray
=============



:Type:	Selection	
:Range:	The settings listed below	
:Default:	No	



This option specifies whether CPLEX should calculate an unbounded ray once CPLEX detects that the model is unbounded. The unbounded ray is passed to AIMMS instead of the normal level values for the variables. Possible values of this option are:



    *	No
    *	Yes




**Note** 

*	The unbounded ray is only available for LP and RMIP models.
*	If the presolver detects unboundedness (or indicates that the model is InfeasibleOrUnbounded) then the unbounded ray is not available. In that case, turn **Presolve**  off and reoptimize to obtain an unbounded ray.
*	If you are using the barrier optimizer without crossover (see the option **LP Method**) then the unbounded ray is not available. 




**Learn more about** 

*	:ref:`option-CPLEX-lp_method`  
*	:ref:`option-CPLEX-presolve`  
