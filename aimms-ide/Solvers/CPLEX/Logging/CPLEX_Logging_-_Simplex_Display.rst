.. _option-CPLEX-simplex_display:


Simplex Display
===============

 

:Type:	Selection	
:Range:	The settings listed below	
:Default:	At refactorizations	



Determines what CPLEX reports during simplex optimization. The amount of information displayed increases as the option value increases. When set to "None", no iteration messages are issued until the optimal solution is reported. When set to "At Refactorizations", an iteration log message will be issued after each refactorization. Each entry will contain the iteration count and scaled infeasibility or objective value. When set to "Every Iteration", an iteration log message will be issued after each iteration. The names of the variable, slacks and artificials entering and leaving the basis will also be reported. Possible values are:



    *	None
    *	At refactorizations
    *	Every iteration




**Remark** 


The logging information is written to the file 'CPLEX 22.1.sta' if the general solvers option **Solver Listing Messages**  is set to 'All' or 'Remark'. To copy the logging information to the listing file the general solvers option **Solver Listing**  should be set to a value different than 'Never'.The file 'CPLEX 22.1.sta' is placed in the log directory of the AIMMS project.





There is no difference between settings 'All' and 'Remark' for option **Solver Listing Messages**, except that with setting 'All' also information is logged for LP problems solved while calculating shadow price ranges for constraints or value ranges for variables, if a simplex algorithm is used to solved those LP problems, as specified by the option **Sensitivity Method**.





**Learn more about** 

*	:ref:`option-CPLEX-sensitivity_method` 
*	:ref:`option-AIMMS-solver_listing`  
*	:ref:`option-AIMMS-solver_listing_messages`  






