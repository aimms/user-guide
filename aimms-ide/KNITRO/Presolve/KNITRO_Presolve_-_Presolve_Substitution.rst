.. _KNITRO_Presolve_-_Presolve_Substitution:


Presolve Substitution
=====================



**Type**:	Selection	

**Range**:	The settings listed below	

**Default**:	Automatic	



This option determines whether or not to enable the Knitro presolve operation to substitute out variable values when possible. Possible values are:



*	Automatic
*	None
*	Simple
*	All




With the default setting 'Automatic', let Knitro determine whether to substitute out variables when possible (may depend on the algorithm).





With the setting 'None', no variable substitutions are performed.





With the setting 'Simple', simple substitutions involving doubleton equality constraints are enabled.





With the setting 'All', all possible variable substitutions are enabled.





**Learn more about** 

*	:ref:`KNITRO_Presolve_-_Presolve`  
*	:ref:`KNITRO_Presolve_-_Presolve_Substitution_Tolerance`  
