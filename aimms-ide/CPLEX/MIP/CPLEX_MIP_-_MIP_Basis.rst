.. _CPLEX_MIP_-_MIP_Basis:


MIP Basis
=========



**Type** :	Selection	

**Range** :	The settings listed below	

**Default** :	No	



By switching on this option the user can pass a basis to CPLEX for a MIP model that can be used by CPLEX for solving the first LP in the branch-and-bound tree search. The value of the general solvers option **Accept Basis**  should also be set to such a value that the basis will be accepted; if the value of the option **Accept Basis**  is 0 then AIMMS wil not pass a basis to CPLEX.



A side effect of passing a basis to CPLEX is that no presolving and crashing will be performed. In case of a MIP model this will in general lead to a loss of performance. Therefore, the default setting of this option is not to load the basis in case of a MIP. Possible values are:



*	No
*	Yes




**Learn more about** 

*	:ref:`Options_Interface_-_Accept_Basis`  
