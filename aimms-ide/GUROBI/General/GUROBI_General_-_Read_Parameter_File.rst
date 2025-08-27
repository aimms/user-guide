.. _option-GUROBI-read_parameter_file:


Read Parameter File
===================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	No	



This option can be used to read in a file with Gurobi option (parameter) settings. The file should be named 'gurobi.prm' and should be placed in the AIMMS project directory. The option settings in this file overrule the option settings in the AIMMS project. Possible values are:



    *	No
    *	Yes




A Gurobi parameter (PRM) file is used to specify parameter settings. The file consists of parameter-value pairs, each on its own line. Any line that begins with the hash sign (#) is a comment line and is ignored. The following is a simple example:





# Parameter settings


Cuts     2


Heuristics 0.5





**Multi-objective optimization** 


During the solution process of a :ref:`GUROBI_Multi-Objective_Optimization` problem, you may prefer that optimization problems with different priorities are solved with different option settings. Gurobi makes this possible by using parameter files. The parameter file of the first optimization problem, tied to the highest priority (possibly blended) objective, should be named 'gurobi_mo1.prm', the parameter file of the second optimization problem should be named 'gurobi_mo2.prm', etc. You do not have to create a parameter file for every multi-objective optimization pass.





For example, to set the **MIP Relative Optimality Tolerance**  to 10% use:





# Parameter settings


MIPGap     0.1





The parameter settings in the multi-objective parameter files will only affect the corresponding pass of the multi-objective optimization. Thus, for example, if the option **Time Limit**  has been set to 100 for this model, but you use a parameter file to set the option to 10 for a particular multi-objective pass, then the multi-objective optimization will spend at most 10 seconds on that particular pass (and at most 100 seconds in total).





**Concurrent MIP** 


If the option **Concurrent MIP**  is set to a value greater than 1, then by switching on this option you can specify option settings for the different instances in a concurrent MIP run. In that case you have to specify n files, where n is the value of the option **Concurrent MIP** , and the files should be named 'gurobi_inst1.prm', 'gurobi_inst2.prm', etc.





**Note** 

*	The parameter file uses Gurobi names instead of AIMMS names for the options. The :ref:`AIMMS_to_GUROBI_Mapping` can be used to find the Gurobi parameter name corresponding to an option in AIMMS.
*	If the setting of an option was changed in the AIMMS project, and the option is not present in the parameter file, then the AIMMS option setting will be used. In other words, the parameter file does not reset options to their default value if they are not present in the parameter file.




**Learn more about** 

*	:ref:`AIMMS_to_GUROBI_Mapping`  
*	:ref:`option-GUROBI-concurrent_mip` 
*	:ref:`option-AIMMS-mip_relative_optimality_tolerance` 
*	:ref:`GUROBI_Multi-Objective_Optimization` 
*	:ref:`option-AIMMS-time_limit` 
