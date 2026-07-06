.. _option-ODHCPLEX-decomposition:


Decomposition
=============



:Type:	Selection
:Range:	The settings listed below
:Default:	Variable keys



This option specifies the method used by ODH-CPLEX to decompose the model into sub-models. Possible values are:



    *	Automatic
    *	Variable keys
    *	Decomposition




With setting 'Automatic', the decomposition method is automatically determined.

With setting 'Variable keys', each variable is assigned to a separate key.

With setting 'Decomposition', the automatic decomposition method is used.




**Note**

*	This option was added in ODH-CPLEX 8.2.

