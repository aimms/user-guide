.. _option-CPLEX-multi_objective_display:


Multi Objective Display
=======================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	None	



This option decides the level of display during multi-objective optimization. Possible values are:



*	None
*	Summary
*	Subproblems logs




At the 'Summary' level CPLEX will display a summary after each subproblem. At the 'Subproblems logs' level CPLEX will also write logs for each subproblem.





**Remark** 


The logging information is written to the file 'CPLEX 22.1.sta' if the general solvers option **Solver Listing Messages**  is set to 'All' or 'Remark'. To copy the logging information to the listing file the general solvers option **Solver Listing**  should be set to a value different than 'Never'.The file 'CPLEX 22.1.sta' is placed in the log directory of the AIMMS project.





**Learn more about** 

*	:ref:`option-AIMMS-solver_listing`  
*	:ref:`option-AIMMS-solver_listing_messages`  
