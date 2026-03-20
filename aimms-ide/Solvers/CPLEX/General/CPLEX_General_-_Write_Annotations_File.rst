.. _option-CPLEX-write_annotations_file:


Write Annotations File
======================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	No	



By setting this option to 'Yes' a CPLEX annotations file will be written. The file will be named cpx\ *ddddd*\ .ann,
where *ddddd* denotes a 5-digit sequence number. Annotations files are written only if one of the options
**LP File**, **MPS** or **Sav File** is set to 'At the first solve' (in which case a annotations file is
written for the first solve) or 'At every solve' (in which case annotations files for every solve are written).

Possible values of this option are:

    *	No
    *	Yes


Annotation files can (only) be used to write the specified decomposition (of the variables) in the Benders decomposition
algorithm, as controlled by the option **Benders Strategy**.


**Learn more about** 

*	:doc:`../Benders/CPLEX_Benders_-_Benders_Strategy` 
*	:doc:`CPLEX_General_-_LP_File`  
*	:doc:`CPLEX_General_-_MPS`  
*	:doc:`CPLEX_General_-_Sav_File`  
