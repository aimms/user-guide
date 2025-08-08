.. _CPLEX_General_-_Read_Parameter_File:


Read Parameter File
===================



**Type** :	Selection	

**Range** :	The settings listed below	

**Default** :	No	



This option can be used to read in a file with CPLEX option (parameter) settings. The file should be named 'cplex.prm' and should be placed in the AIMMS project directory. Possible values are:



*	No
*	Yes
*	Overrule




With setting 'Yes' the parameter file is read but the option settings in the parameter file will be overruled by non-default option settings in the AIMMS project. With setting 'Overrule' the option settings in the parameter file overrule the option settings in the AIMMS project.





A CPLEX parameter (PRM) file is used to specify parameter settings. The file consists of parameter-value pairs, each on its own line. Any line that begins with the hash sign (#) is a comment line and is ignored. The following is a simple example:





CPLEX Parameter File Version 22.1.0.0


CPX_PARAM_PERIND    1


CPX_PARAM_EPPER     3.45000000000000e-06


CPX_PARAM_STARTALG   2





The first line is mandatory. The name for the parameters used should be the CPLEX C API names as can be found in the:ref:`CPLEX_AIMMS_to_CPLEX_Mapping`  from AIMMS option names to CPLEX parameter names.





**Note** 

*	With setting 'Overrule' the parameter file resets options not present in the parameter file to their default CPLEX value. So, if an option was set to a non-default value in the AIMMS project and it is not present in the parameter file, then the default value will be used by CPLEX.




**Multi-objective optimization** 


During the solution process of a :ref:`CPLEX_Multi_Objective_Optimization`  problem, you may prefer that optimization problems with different priorities are solved with different option settings. CPLEX makes this possible by using parameter files. The parameter file of the first optimization problem, corresponding to the highest priority (possibly blended) objective, should be named 'cplex_mo1.prm', the parameter file of the second optimization problem should be named 'cplex_mo2.prm', etc. You do not have to create a parameter file for every multi-objective optimization pass.





For example, to set the **MIP Relative Optimality Tolerance**  to 10% use:





CPLEX Parameter File Version 22.1.0.0


CPX_PARAM_EPGAP    0.1





The parameter settings in the multi-objective parameter files will only affect the corresponding pass of the multi-objective optimization. Thus, for example, if the option **Time Limit**  has been set to 100 for this model, but you use a parameter file to set the option to 10 for a particular multi-objective pass, then the multi-objective optimization will spend at most 10 seconds on that particular pass (and at most 100 seconds in total). The option **Deterministic Time Limit**  behaves in a similar way.





**Note** 

*	The parameter file uses CPLEX names instead of AIMMS names for the options. The :ref:`CPLEX_AIMMS_to_CPLEX_Mapping`  can be used to find the CPLEX parameter name corresponding to an option in AIMMS.
*	The option **Parallel Mode**  cannot be changed during the solution process of a multi-objective optimization problem; it will be ignored when present in a multi-objective parameter file.
*	With setting 'Overrule' the parameter files specifying different option settings for multi-objective optimization will be ignored.




**Learn more about** 

*	:ref:`CPLEX_AIMMS_to_CPLEX_Mapping`  
*	:ref:`CPLEX_General_-_Deterministic_Time_Limit` 
*	:ref:`Options_MIP_Options_-_MIP_Relative_Opt` 
*	:ref:`CPLEX_Multi_Objective_Optimization` 
*	:ref:`CPLEX_Par_-_Parallel_Mode` 
*	:ref:`Options_Stop_Criteria_-_Time_Limit` 
