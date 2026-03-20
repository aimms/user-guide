.. _option-ODHCPLEX-write_decomposition_file:


Write Decomposition File
========================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	No	



When this option is switched on, a decomposition file is generated containing the model structure specified in the loaded model. The data will be written to a file called cpxddddd.dec, where ddddd denotes a 5-digit sequence number. Possible values are:



    *	No
    *	Yes




Decomposition files are written only if one of the options **LP File**, **MPS**  or **Sav File**  is set to 'At the first solve' (in which case a decomposition file is written for the first solve) or 'At every solve' (in which case decomposition files for every solve are written).





**Note** 

*	The decomposition file will only be written if a decomposition has been specified in the model, using the routine GMP::Column::SetDecomposition, as explained in the section :doc:`ODH_-_Specifying_Model_Structure <../ODH_-_Specifying_Model_Structure>`.




**Learn more about** 

*	:doc:`ODH_XGeneral_-_LP_File <../CPLEX General/ODH_XGeneral_-_LP_File>`  
*	:doc:`ODH_XGeneral_-_MPS <../CPLEX General/ODH_XGeneral_-_MPS>`  
*	:doc:`ODH_XGeneral_-_Sav_File <../CPLEX General/ODH_XGeneral_-_Sav_File>`  
*	:doc:`ODH_-_Specifying_Model_Structure <../ODH_-_Specifying_Model_Structure>` 



