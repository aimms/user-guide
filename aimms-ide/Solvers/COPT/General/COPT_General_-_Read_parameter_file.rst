.. _option-COPT-read_parameter_file:


Read Parameter File
===================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	No	



This option can be used to read in a file with COPT option (parameter) settings. The file should be named copt.prm' and should be placed in the AIMMS project directory. The option settings in this file overrule the option settings in the AIMMS project. Possible values are:



    *	No
    *	Yes




The parameter file uses COPT names instead of AIMMS names for the options. The :ref:`COPT_to_AIMMS_Mapping`  can be used to find the COPT parameter name corresponding to an option in AIMMS.





**Note** 

*	If the setting of an option was changed in the AIMMS project, and the option is not present in the parameter file, then the AIMMS option setting will be used. In other words, the parameter file does not reset options to their default value if they are not present in the parameter file.




**Learn more about** 

*	:ref:`COPT_to_AIMMS_Mapping` 
