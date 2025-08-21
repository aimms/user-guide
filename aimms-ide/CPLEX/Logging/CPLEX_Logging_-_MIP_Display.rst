.. _option-CPLEX-mip_display:


MIP Display
===========



:Type:	Selection	
:Range:	The settings listed below	
:Default:	None	



This option determines what CPLEX reports to the log file during mixed integer optimization. A setting of "None" causes no node log to be displayed until the optimal solution is found.



A setting of "Display integer feasible solutions" displays an entry for each integer feasible solution found. Each entry contains the objective function value, the node count, the number of unexplored nodes in the tree, and the current optimality gap.



A setting of "Display each nth node" also generates an entry for every nth node (where n is the setting of the **MIP Interval**  option). A setting of "Nth node + info on node cuts" additionally generates an entry for every nth node giving the number of cuts added to the problem for the previous n nodes. A setting of "Nth node + LP display for root node" additionally generates entries for the LP root relaxation according to the setting of the option **Simplex Display** (or the option **Barrier Display** ). A setting of "Nth node + LP display for all nodes" additionally generates entries for the LP subproblems, also according to the setting of the option **Simplex Display** (or the option **Barrier Display** ).



Possible values are:



*	None
*	Display integer feasible solutions
*	Display each nth node
*	Nth node + info on node cuts
*	Nth node + LP display for root node
*	Nth node + LP display for all nodes




**Remark** 


The logging information is written to the file 'CPLEX 22.1.sta' if the general solvers option **Solver Listing Messages**  is set to 'All' or 'Remark'. To copy the logging information to the listing file the general solvers option **Solver Listing**  should be set to a value different than 'Never'.The file 'CPLEX 22.1.sta' is placed in the log directory of the AIMMS project.





The difference between settings 'All' and 'Remark' for option **Solver Listing Messages**  is that for setting 'All' also information about branching variables is printed, if the **MIP Display**  is at least 'Display each nth node'. However, information about branching variables is only printed if the option **MIP Search Strategy**  is set to 'Apply branch-and-cut'.





**Learn more about** 

*	:ref:`option-CPLEX-barrier_display` 
*	:ref:`option-CPLEX-mip_interval` 
*	:ref:`option-CPLEX-mip_search_strategy` 
*	:ref:`option-CPLEX-simplex_display` 
*	:ref:`Options_Solver_Specific_-_Solver_Listi`  
*	:ref:`Options_Solver_Specific_-_Solver_List1`  



