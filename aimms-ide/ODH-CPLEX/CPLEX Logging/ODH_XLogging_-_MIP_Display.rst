.. _ODH-CPLEX_XLogging_-_MIP_Display:


MIP Display
===========



**Type**:	Selection	

**Range**:	The settings listed below	

**Default**:	None	



This option determines what logging information CPLEX reports during mixed integer optimization. A setting of "None" causes no logging to be displayed until the optimal solution is found.



A setting of "Display integer feasible solutions" displays an entry for each integer feasible solution found. Each entry contains the objective function value, the node count, the number of unexplored nodes in the tree, and the current optimality gap.



A setting of "Display each nth node" also generates an entry for every nth node (where n is the setting of the **MIP Interval**  option). A setting of "Nth node + info on node cuts" additionally generates an entry for every nth node giving the number of cuts added to the problem for the previous n nodes. A setting of "Nth node + LP display for root node" additionally generates entries for the LP root relaxation according to the setting of the option **Simplex Display**  (or the option **Barrier Display** ). A setting of "Nth node + LP display for all nodes" additionally generates entries for the LP subproblems, also according to the setting of the option **Simplex Display** (or the option **Barrier Display** ).



Possible values are:



*	None
*	Display integer feasible solutions
*	Display each nth node
*	Nth node + info on node cuts
*	Nth node + LP display for root node
*	Nth node + LP display for all nodes




The logging information is written to the AIMMS message window if the general solvers option **Solver Window Messages**  is set to 'All'.





**Note** 

*	Logging information is only reported if the option **Status Display**  is switched on.
*	The logging information is written to the status file 'ODH-CPLEX 5.3.log' if the general solvers option **Solver Listing Messages**  is set to 'All'. The status file is placed in the log directory of the current project.
*	The logging information is written to the AIMMS message window if the general solvers option **Solver Window Messages**  is set to 'All'.




**Learn more about** 

*	:ref:`ODH-CPLEX_XLogging_-_Barrier_Display` 
*	:ref:`ODH-CPLEX_XLogging_-_MIP_Display` 
*	:ref:`ODH-CPLEX_XLogging_-_Simplex_Display` 
*	:ref:`Options_Solver_Specific_-_Solver_List1`   (General solvers option)
*	:ref:`Options_Solver_Specific_-_Solver_Windo`   (General solvers option)
*	:ref:`ODH-CPLEX_Logging_-_Status_Display` 



