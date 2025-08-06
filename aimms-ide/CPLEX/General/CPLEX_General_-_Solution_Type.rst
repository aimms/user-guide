.. _CPLEX_General_-_Solution_Type:


Solution Type
=============



**Type** :	Selection	

**Range** :	The settings listed below	

**Default** :	Automatic	



This option specifies the type of solution (basic or non basic) that CPLEX attempts to compute for a linear program (LP) or for a quadratic program (QP). In this context, basic means having to do with the basis, and non basic applies to the variables and constraints not participating in the basis. Possible values are:



*	Automatic
*	Basic
*	Nonbasic




When the value of this option is 'Automatic' or 'Basic', CPLEX seeks a basic solution, that is, a solution that includes a basis with a basic status for variables and constraints.





When the value of this option is 'Nonbasic', CPLEX seeks a pair of primal-dual solution vectors. This setting does not prevent CPLEX from producing status information, but in seeking a pair of primal-dual solution vectors, CPLEX possibly may not produce basic status information; that is, it is possible that CPLEX does not produce status information about which variables and constraints participate in the basis at this setting.





**Note** 

*	If the setting 'Nonbasic' is chosen, sensitivity information for objective coefficient ranges for variables and right-hand-side ranges for constraints will not be available because a basic solution is required to calculate those ranges. Also, the sensitivity information for value ranges for variables and shadow price ranges for constraints will be meaningless.
*	If CPLEX uses the barrier optimizer, as controlled by the option **LP Method** , then a crossover is performed at the end of a barrier optimization. The option **Barrier Crossover Algorithm**  determines which algorithm CPLEX will use for the crossover.




**Learn more about** 

*	:ref:`CPLEX_Barrier_-_Barrier_cross` 
*	:ref:`CPLEX_General_-_LP_Method` 
