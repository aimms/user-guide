.. _ODH-CPLEX_XLogging_-_Barrier_Display:


Barrier Display
===============



**Type** :	Selection	

**Range** :	The settings listed below	

**Default** :	None	



The setting of this option determines the level of barrier progress information to be displayed while solving a mixed integer problem. At the default level, no progress information is displayed. At the level "Normal", "normal" setup and iteration information is displayed (see the section "Barrier Input & Output" in Chapter 2 of the CPLEX documentation for a complete interpretation of normal display information). At a setting of "Diagnostics", additional diagnostic information is displayed which may be useful when seeking technical support. Possible values are:



*	None
*	Normal
*	Diagnostics




**Note** 

*	Logging information is only reported if the option **Status Display**  is switched on.
*	Barrier logging is only reported if the option **MIP Display**  is set to 'Nth node + LP display for root node' or 'Nth node + LP display for all nodes'.
*	The logging information is written to the status file 'ODH-CPLEX 5.3.log' if the general solvers option **Solver Listing Messages**  is set to 'All'. The status file is placed in the log directory of the current project.
*	The logging information is written to the AIMMS message window if the general solvers option **Solver Window Messages**  is set to 'All'.




**Learn more about** 

*	:ref:`ODH-CPLEX_XLogging_-_MIP_Display` 
*	:ref:`Options_Solver_Specific_-_Solver_List1`   (General solvers option)
*	:ref:`Options_Solver_Specific_-_Solver_Windo`   (General solvers option)
*	:ref:`ODH-CPLEX_Logging_-_Status_Display` 






