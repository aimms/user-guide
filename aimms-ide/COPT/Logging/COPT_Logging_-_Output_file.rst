.. _COPT_Logging_-_Output_file:


Output File
===========



**Type**:	Selection	

**Range**:	The settings listed below	

**Default**:	No	



This option can be used to activate the generation of a COPT output file. The output file is named "copt.log" and is placed in the log-directory of the current project. Possible values are:



*	No
*	Yes




**Remark** 


The logging information is written to the output file only if the general solvers option **Solver Listing Messages**  is set to 'All' or 'Remark'. To copy the logging information to the listing file the general solvers option **Solver Listing**  should be set to a value different than 'Never'.





There is no difference between settings 'All' and 'Remark' for option **Solver Listing Messages** , except that with setting 'All' also information is logged for LP problems solved while calculating shadow price ranges for constraints or value ranges for variables; see the option **Sensitivity Method** .





**Learn more about** 

*	:ref:`COPT_General_-_Sensitivity_method` 
*	:ref:`Options_Solver_Specific_-_Solver_Listi`  
*	:ref:`Options_Solver_Specific_-_Solver_List1`  



