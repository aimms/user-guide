.. _GUROBI_General_-_Farkas_Infeasibility_Proof:


Farkas Infeasibility Proof
==========================



**Type**:	Selection	

**Range**:	The settings listed below	

**Default**:	No	



This option specifies whether Gurobi should retrieve a Farkas infeasibility proof once Gurobi detects that the model is infeasible. The Farkas infeasibility proof provides a dual unbounded vector. Adding this vector into any feasible solution to the dual model yields a new solution that is also feasible but improves the dual objective. This vector is passed to AIMMS instead of the normal level values for the constraints. Note that the general solvers option **Always Store Constraint Levels**  should be switched on.



The magnitude of the infeasibility violation in the Farkas infeasibility proof is stored in the .SumOfInfeasibilities suffix of the math program.



Possible values of this option are:



*	No
*	Yes




**Note** 

*	The Farkas infeasibility proof is only available for LP and RMIP models.
*	If the presolver detects infeasibility (or indicates that the model is InfeasibleOrUnbounded) then the Farkas infeasibility proof is not available. In that case, turn **Presolve**  off and reoptimize to obtain the Farkas infeasibility proof.
*	If you are using the barrier optimizer without crossover (see the options **Method**  and **Barrier Crossover** ) then the Farkas infeasibility proof is not available. 




**Learn more about** 

*	:ref:`Options_Sensitivity_-_Always_Store_Con`  
*	:ref:`GUROBI_Barrier_-_Barrier_Crossover`  
*	:ref:`GUROBI_General_-_Method`  
*	:ref:`GUROBI_Presolve_-_Presolve`  
