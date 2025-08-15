.. _CPOPT_Preprocessing_-_Preprocess_table_constraints:


Preprocess table constraints
============================



**Type**:	Selection	

**Range**:	The settings listed below	

**Default**:	On	



This option determines whether table constraints should be preprocessed. Possible values are:



*	Off
*	On




Table constraints are constraints that use the IN operator to explicitly list all tuples that are allowed for some combination of variables. For example:





 CONSTRAINT:


   identifier : DomRestr2


   definition : (eV1, eV2, eV3) in ThreeDimRelation


   comment  : "ThreeDimRelation contains all allowed tuples" ;





See the Language Reference for more information about table constraints.

