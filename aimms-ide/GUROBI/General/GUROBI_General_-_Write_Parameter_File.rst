.. _option-GUROBI-write_parameter_file:


Write Parameter File
====================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	No	



By setting this option to 'Yes' a Gurobi parameter file will be written. The file will be named gurobi.prm. Possible values of this option are:



*	No
*	Yes




A Gurobi parameter (PRM) file is used to specify parameter settings. The file consists of parameter-value pairs, each on its own line.





The parameters are printed using the Gurobi C API names as can be found in the:ref:`AIMMS_to_GUROBI_Mapping` from AIMMS option names to Gurobi parameter names.





**Note** 

*	Only parameters (options) with non-default values according to Gurobi will be printed.
