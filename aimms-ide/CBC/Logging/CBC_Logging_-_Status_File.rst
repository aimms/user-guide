.. _CBC_Logging_-_Status_File:


Status file
===========



**Type** :	Selection	

**Range** :	The settings listed below	

**Default** :	Off	



This option can be used to activate the generation of a CBC output file. The status file is named "cbc.sta" and is placed in the log-directory of the current project. Possible values are:



*	Off
*	File
*	Stdout




Setting 'Stdout' means that CBC will write to standard output.





**Remark** 


The logging information is written if the general solvers option **Solver Listing Messages**  is set to 'All'. To copy the logging information to the listing file the general solvers option **Solver Listing**  should be set to a value different than 'Never'.





**Learn more about** 

*	:ref:`Options_Solver_Specific_-_Solver_Listi`  
*	:ref:`Options_Solver_Specific_-_Solver_List1`  
