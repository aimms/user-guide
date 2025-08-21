.. _option-CPLEX-cmd_file:


Cmd File
========



:Type:	Selection	
:Range:	The settings listed below	
:Default:	No	



By setting this option to 'Yes', command files will be generated. These command files can be used as input to the CPLEX Interactive Optimizer. Command files are written only if one of the options **LP File,**  **MPS**  or **Sav File**  is set to 'At the first solve' (in which case a cmd file is written for the first solve) or 'At every solve' (in which case cmd files for every solve are written).



Possible values of this option are:



*	No
*	Yes




The command file will be named cpxddddd.cmd, where ddddd denotes a 5-digit sequence number.





**Learn more about** 

*	:ref:`option-CPLEX-lp_file`  
*	:ref:`option-CPLEX-mps`  
*	:ref:`option-CPLEX-sav_file`  



