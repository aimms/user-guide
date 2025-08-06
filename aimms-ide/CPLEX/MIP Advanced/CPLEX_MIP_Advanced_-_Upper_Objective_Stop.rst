.. _CPLEX_MIP_Advanced_-_Upper_Objective_Stop:


Upper Objective Stop
====================



**Type** :	Floating point number	

**Range** :	[-1e75, 1e75)	

**Default** :	1e75	



In a maximization MILP or MIQP, CPLEX will abort the optimization process as soon it finds a solution of value greater than or equal to the specified value for this option.



This option is ignored if the problem is multi-objective.



**Learn more about** 

*	:ref:`CPLEX_MIP_Advanced_-_Lower_Objective_Stop` 



