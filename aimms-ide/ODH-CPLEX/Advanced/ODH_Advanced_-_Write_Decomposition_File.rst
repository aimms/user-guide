.. _ODH-CPLEX_Advanced_-_Write_Decomposition_File:


Write Decomposition File
========================



**Type** :	Selection	

**Range** :	The settings listed below	

**Default** :	No	



When this option is switched on, a decomposition file is generated containing the model structure specified in the loaded model. The data will be written to a file called cpxddddd.dec, where ddddd denotes a 5-digit sequence number. Possible values are:



*	No
*	Yes




Decomposition files are written only if one of the options **LP File** , **MPS**  or **Sav File**  is set to 'At the first solve' (in which case a decomposition file is written for the first solve) or 'At every solve' (in which case decomposition files for every solve are written).





**Note** 

*	The decomposition file will only be written if a decomposition has been specified in the model, using the routine GMP::Column::SetDecomposition, as explained in the section :ref:`ODH-CPLEX_-_Specifying_Model_Structure` .




**Learn more about** 

*	:ref:`ODH-CPLEX_XGeneral_-_LP_File`  
*	:ref:`ODH-CPLEX_XGeneral_-_MPS`  
*	:ref:`ODH-CPLEX_XGeneral_-_Sav_File`  
*	:ref:`ODH-CPLEX_-_Specifying_Model_Structure` 



