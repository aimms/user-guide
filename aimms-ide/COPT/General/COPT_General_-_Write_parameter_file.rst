.. _option-COPT-write_parameter_file:


Write Parameter File
====================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	No	



By setting this option to 'Yes' a COPT parameter file will be written. The file will be named coptddddd.prm, where ddddd denotes a 5-digit sequence number. Parameter files are written only if the option **MPS**  is set to a non-default value. Possible values are:



*	No
*	Yes




The parameter file uses COPT names instead of AIMMS names for the options. The :ref:`COPT_to_AIMMS_Mapping`  can be used to find the COPT parameter name corresponding to an option in AIMMS.





**Learn more about** 

*	:ref:`option-COPT-mps` 
*	:ref:`COPT_to_AIMMS_Mapping` 
