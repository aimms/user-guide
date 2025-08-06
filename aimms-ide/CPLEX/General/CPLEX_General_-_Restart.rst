.. _CPLEX_General_-_Restart:


Restart
=======



**Type** :	Selection	

**Range** :	The settings listed below	

**Default** :	No	



In some cases one might want to interrupt the current solve and continue it later on. In order to restart the solver, essential information about the current solution should be saved in a file. Furthermore, the solver should be told to read this data and continue the solve. This option can be used to generate the necessary restart information and to restart the solver.



When this option is set to "Yes", the solver will restart a problem if the solution file cpxddddd.sol exists. The number ddddd represents the current value of the option **Restart File Number** . After the solve the file cpxddddd.sol will be generated. Possible values are:



*	No
*	Yes




**Learn more about** 

*	:ref:`CPLEX_General_-_Restart_File_Nr` 



