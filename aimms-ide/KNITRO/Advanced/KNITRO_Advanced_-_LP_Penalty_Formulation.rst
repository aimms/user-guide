.. _KNITRO_Advanced_-_LP_Penalty_Formulation:


LP Penalty Formulation
======================



**Type** :	Selection	

**Range** :	The settings listed below	

**Default** :	All	



This option indicates whether to use a penalty formulation for linear programming subproblems in the Knitro Active Set or SQP algorithms. Possible values are:



*	All
*	Nonlinear
*	Dynamic




With setting 'All' all constraints are penalized. With setting 'Nonlinear' only the nonlinear constraints are penalized. With setting 'Dynamic' Knitro dynamically chooses which constraints to penalize.





This option has no effect on the Interior/Direct and Interior/CG algorithms.




