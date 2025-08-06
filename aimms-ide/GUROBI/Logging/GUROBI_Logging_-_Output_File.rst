.. _GUROBI_Logging_-_Output_File:


Output File
===========



**Type** :	Selection	

**Range** :	The settings listed below	

**Default** :	No	



This option can be used to activate the generation of a Gurobi output file. The output file is named "gurobi.log" and is placed in the log-directory of the current project. Possible values are:



*	No
*	Yes




**Remark** 


The logging information is written to the output file only if the general solvers option **Solver Listing Messages**  is set to 'All' or 'Remark'. To copy the logging information to the listing file the general solvers option **Solver Listing**  should be set to a value different than 'Never'.





There is no difference between settings 'All' and 'Remark' for option **Solver Listing Messages** , except that with setting 'All' also information is logged for LP problems solved while calculating shadow price ranges for constraints or value ranges for variables; see the option **Sensitivity Method** .





**Note** 

*	Set the option **Display Solution Quality**  to let Gurobi print solution quality statistics in the Gurobi output file.




**Learn more about** 

*	:ref:`GUROBI_Logging_-_Display_Solution_Quality` 
*	:ref:`GUROBI_Logging_-_Output_File_Display_Interval` 
*	:ref:`GUROBI_General_-_Sensitivity_Method` 
*	:ref:`Options_Solver_Specific_-_Solver_Listi`  
*	:ref:`Options_Solver_Specific_-_Solver_List1`  



