.. _option-ODHCPLEX-strict_deterministic:


Strict Deterministic
====================



:Type:	Selection
:Range:	The settings listed below
:Default:	No



This option specifies whether ODH-CPLEX terminates deterministically when the solution improvement heuristic finishes. Possible values are:



    *	No
    *	Yes




With setting 'No', ODH-CPLEX terminates as soon as possible, which can violate determinism.

With setting 'Yes', ODH-CPLEX terminates deterministically.




**Note**

*	This option was added in ODH-CPLEX 8.2.

