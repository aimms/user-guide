.. _CPLEX_Logging_-_Tuning_Display:


Tuning Display
==============



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Minimal	



This option specifies the level of information reported by the tuning tool as it works. Possible values are:



*	Off
*	Minimal
*	Standard
*	Exhaustive




Use settings 'Standard' and 'Exhaustive' to display the option settings that the tuning tool is trying.





**Remark** 


The logging information is written to the file 'CPLEX 22.1.sta' if the general solvers option **Solver Listing Messages**  is set to 'All' or 'Remark'. To copy the logging information to the listing file the general solvers option **Solver Listing**  should be set to a value different than 'Never'.The file 'CPLEX 22.1.sta' is placed in the log directory of the AIMMS project.





**Learn more about** 

*	:ref:`Options_Solver_Specific_-_Solver_Listi`  
*	:ref:`Options_Solver_Specific_-_Solver_List1`  
*	:ref:`CPLEX_Tuning_Tool` 
