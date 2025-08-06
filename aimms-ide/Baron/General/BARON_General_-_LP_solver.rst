

.. _Baron_General_-_LP_solver:


LP solver
=========



**Type** :	Selection	

**Range** :	The settings listed below	

**Default** :	Automatic	



This option specifies the LP solver to be used. At the default setting AIMMS chooses the LP solver based on license information; if the AIMMS license allows CPLEX then CPLEX will be chosen, otherwise the COIN-OR solver CLP will be selected. Possible values are:



*	Automatic
*	CPLEX
*	CLP
*	None




**Note** 

*	AIMMS will generate an execution error if an LP solver is chosen that is not allowed by the AIMMS license.



