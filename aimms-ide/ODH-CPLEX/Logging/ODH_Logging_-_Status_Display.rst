.. _ODH-CPLEX_Logging_-_Status_Display:


Status Display
==============



:Type:	Selection	
:Range:	The settings listed below	
:Default:	No	



This option can be used to activate the generation of logging messages by ODH-CPLEX, if also one of the general solvers options **Solver Listing Messages**  or **Solver Window Messages**  is set to 'All'. Possible values are:



*	No
*	Yes




The logging information is written to the status file 'ODH-CPLEX 5.3.log' if the general solvers option **Solver Listing Messages**  is set to 'All'. The status file is placed in the log directory of the current project.





The logging information is written to the AIMMS message window if the general solvers option **Solver Window Messages**  is set to 'All'.





**Note** 

*	By default only logging for the ODH engine will be printed in the status file. You can also enable CPLEX logging in this status file by setting the option **MIP Display** .
*	It is not possible to copy the ODH-CPLEX logging information to the listing file by using the general solvers option **Solver Listing** .




**Learn more about** 

*	:ref:`ODH-CPLEX_XLogging_-_MIP_Display` 
*	:ref:`Options_Solver_Specific_-_Solver_Listi`   (General solvers option)
*	:ref:`Options_Solver_Specific_-_Solver_List1`   (General solvers option)
*	:ref:`Options_Solver_Specific_-_Solver_Windo`   (General solvers option)
