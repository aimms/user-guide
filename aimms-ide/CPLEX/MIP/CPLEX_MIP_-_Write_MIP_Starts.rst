.. _option-CPLEX-write_mip_starts:


Write MIP Starts
================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	No	



By setting this option to 'Yes' a CPLEX file with MIP starts will be written, but only if one or more MIP starts have been specified. The file will be named cpxddddd.mst, where ddddd denotes a 5-digit sequence number. The MIP Start file is written only if one of the options **LP File,**  **MPS**  or **Sav File**  is set to 'At the first solve' (in which case the MIP Start file is written for the first solve) or 'At every solve' (in which case MIP Start files for every solve are written).



Possible values of this option are:



    *	No
    *	Yes




**Learn more about** 

*	:ref:`option-CPLEX-lp_file`  
*	:ref:`option-CPLEX-mps`  
*	:ref:`option-CPLEX-sav_file`  
