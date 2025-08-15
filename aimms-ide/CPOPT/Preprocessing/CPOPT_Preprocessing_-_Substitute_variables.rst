.. _CPOPT_Preprocessing_-_Substitute_variables:


Substitute variables
====================



**Type**:	Selection	

**Range**:	The settings listed below	

**Default**:	Off	



This option determines whether so called doubletons should be removed. Possible values are:



*	Off
*	On




A doubleton is defined by two variables that appear in a constraint of the form αX = αY, where X and Y are two variables and α is a value unequal to 0. If such a doubleton exists then Y can be replaced by X in all constraints, and variable Y and the constraint αX = αY can be deleted.





If this option is switched on then doubletons will be removed. However, if the variables X and Y of a doubleton appear together in any constraint other than the αX = αY constraint, then the doubleton will not be removed.

