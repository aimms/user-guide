.. _option-ODHCPLEX-simplex_display:


Simplex Display
===============

 

:Type:	Selection	
:Range:	The settings listed below	
:Default:	At refactorizations	



Determines what CPLEX reports during simplex optimization while solving a mixed integer problem. The amount of information displayed increases as the option value increases. When set to "None", no iteration messages are issued until the optimal solution is reported. When set to "At Refactorizations", an iteration log message will be issued after each refactorization. Each entry will contain the iteration count and scaled infeasibility or objective value. When set to "Every Iteration", an iteration log message will be issued after each iteration. The names of the variable, slacks and artificials entering and leaving the basis will also be reported. Possible values are:



    *	None
    *	At refactorizations
    *	Every iteration




**Note** 

*	Logging information is only reported if the option **Status Display**  is switched on.
*	Simplex logging is only reported if the option **MIP Display**  is set to 'Nth node + LP display for root node' or 'Nth node + LP display for all nodes'.
*	The logging information is written to the status file 'ODH-CPLEX 5.3.log' if the general solvers option **Solver Listing Messages**  is set to 'All'. The status file is placed in the log directory of the current project.
*	The logging information is written to the AIMMS message window if the general solvers option **Solver Window Messages**  is set to 'All'.




**Learn more about** 

*	:ref:`option-ODHCPLEX-mip_display` 
*	:ref:`option-AIMMS-solver_listing_messages`   (General solvers option)
*	:ref:`option-AIMMS-solver_window_messages`   (General solvers option)
*	:ref:`option-ODHCPLEX-status_display` 






