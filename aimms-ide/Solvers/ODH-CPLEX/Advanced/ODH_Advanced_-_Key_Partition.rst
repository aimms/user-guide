.. _option-ODHCPLEX-key_partition:


Key Partition
=============



:Type:	Selection
:Range:	The settings listed below
:Default:	Off



This option controls the use of solver partition information. Possible values are:



    *	Off
    *	Keys from solver partition
    *	Keys to sub-solver partition




With setting 'Keys from solver partition', solver partition information is used to generate keys.

With setting 'Keys to sub-solver partition', keys are used to generate sub-solver partition information.




**Note**

*	This option was added in ODH-CPLEX 8.2.

