.. _ODH-CPLEX_XLogging_-_MIP_Interval:


MIP Interval
============

 

**Type** :	Integer	

**Range** :	{-2147483647 .. 2147483647}	

**Default** :	0	



This option controls the frequency of the node logging when the option **MIP Display**  is set to "Integer + each nth node" or "All nodes + LP log". If the value of this option is a positive integer n, then only every nth node, plus all integer feasible nodes, will be logged. This option is useful for monitoring the progress of a problem that requires many nodes to solve.



When the value is a negative integer n, CPLEX displays new incumbents, and the negative value determines how much processing CPLEX does before it displays a new line in the node log. A negative value close to 0 means that CPLEX displays new lines in the log frequently. A negative value far from 0 means that CPLEX displays new lines in the log less frequently. In other words, a negative value of this parameter contracts or dilates the interval at which CPLEX displays information in the node log.



At the default value of 0, CPLEX decides the frequency to log nodes.



**Note** 

*	Logging information is only reported if the option **Status Display**  is switched on.
*	The logging information is written to the status file 'ODH-CPLEX 5.3.log' if the general solvers option **Solver Listing Messages**  is set to 'All'. The status file is placed in the log directory of the current project.
*	The logging information is written to the AIMMS message window if the general solvers option **Solver Window Messages**  is set to 'All'.




**Learn more about** 

*	:ref:`ODH-CPLEX_XLogging_-_MIP_Display` 
*	:ref:`Options_Solver_Specific_-_Solver_List1`   (General solvers option)
*	:ref:`Options_Solver_Specific_-_Solver_Windo`   (General solvers option)
*	:ref:`ODH-CPLEX_Logging_-_Status_Display` 



