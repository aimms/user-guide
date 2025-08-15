.. _CONOPT_General_-_Model_is_Square:

Model is Square System
======================



**Type**:	Selection	

**Range**:	The settings listed below	

**Default**:	Off	



If this option is turned on, the modeler declares that the model is a square system. This implies that:



*	The number of non-fixed variables (including slack in inequalities) must be equal to the number of constraints,
*	No bounds must be active in the final solution, and
*	The basis selected from the non-fixed variables always must be nonsingular.




Possible values are:




*	Off
*	On



