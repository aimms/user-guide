.. _XA_General_-_Restart:


Restart
=======



**Type** :	Selection	

**Range** :	The settings listed below	

**Default** :	No	



In some cases one might want to interrupt the current solve and continue it later on. In order to restart the solver, essential information about the current solution should be saved in a file. Furthermore, the solver should be told to read this data and continue the solve. This option can be used to generate the necessary restart information and to restart the solver.

When this option is set to yes, the solver will restart when the file xaddddd.bas, where ddddd represents the current value of option **Restart File Number** , exists. In case of a MIP restart, the presence of the files xaddddd.b01 and xaddddd.r01 is also required. Furthermore, at the end of the solve the file xaddddd.bas will be generated. If the solver is interrupted during a MIP search, the files xaddddd.b01 and xaddddd.r01 will be generated too. These two files contain information for restarting the MIP search.

Possible values are:



*	No
*	Yes




**Learn more about** 

*	:ref:`XA_General_-_Restart_File_Number`  



