.. _CPLEX_MIP_-_Write_MIP_Starts:


Write MIP Starts
================



**Type**:	Selection	

**Range**:	The settings listed below	

**Default**:	No	



By setting this option to 'Yes' a CPLEX file with MIP starts will be written, but only if one or more MIP starts have been specified. The file will be named cpxddddd.mst, where ddddd denotes a 5-digit sequence number. The MIP Start file is written only if one of the options **LP File,**  **MPS**  or **Sav File**  is set to 'At the first solve' (in which case the MIP Start file is written for the first solve) or 'At every solve' (in which case MIP Start files for every solve are written).



Possible values of this option are:



*	No
*	Yes




**Learn more about** 

*	:ref:`CPLEX_General_-_LP_File`  
*	:ref:`CPLEX_General_-_MPS`  
*	:ref:`CPLEX_General_-_Sav_File`  
