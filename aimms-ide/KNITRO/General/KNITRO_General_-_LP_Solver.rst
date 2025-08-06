.. _KNITRO_General_-_LP_Solver:


LP Solver
=========



**Type** :	Selection	

**Range** :	The settings listed below	

**Default** :	Internal	



This option indicates which linear programming (simplex) solver the Active-Set and SQP algorithms should use when solving internal LP subproblems. Possible values are:



*	Internal
*	CPLEX




For setting 'Internal' Knitro uses its own LP solver.





**Note** 

*	CPLEX can only be used if the AIMMS license includes CPLEX.




**Learn more about** 

*	:ref:`KNITRO_General_-_Algorithm` 
