.. _CPLEX_Logging_-_MIP_Interval:


MIP Interval
============

 

**Type** :	Integer	

**Range** :	{-2147483647 .. 2147483647}	

**Default** :	0	



This option controls the frequency of the node logging when the option **MIP Display**  is set to "Integer + each nth node" or "All nodes + LP log". If the value of this option is a positive integer n, then only every nth node, plus all integer feasible nodes, will be logged. This option is useful for monitoring the progress of a problem that requires many nodes to solve.



When the value is a negative integer n, CPLEX displays new incumbents, and the negative value determines how much processing CPLEX does before it displays a new line in the node log. A negative value close to 0 means that CPLEX displays new lines in the log frequently. A negative value far from 0 means that CPLEX displays new lines in the log less frequently. In other words, a negative value of this parameter contracts or dilates the interval at which CPLEX displays information in the node log.



At the default value of 0, CPLEX decides the frequency to log nodes.



**Remark** 

The logging information is written to the file 'CPLEX 22.1.sta' if the general solvers option **Solver Listing Messages**  is set to 'All'. To copy the logging information to the listing file the general solvers option **Solver Listing**  should be set to a value different than 'Never'.The file 'CPLEX 22.1.sta' is placed in the log directory of the AIMMS project.



**Learn more about** 

*	:ref:`CPLEX_Logging_-_MIP_Display` 
*	:ref:`Options_Solver_Specific_-_Solver_Listi`  
*	:ref:`Options_Solver_Specific_-_Solver_List1`  



