

.. _option-AIMMS-database_translate_0_to_zero:


Database Translate 0 to Zero
============================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Never	



When an explicit 0 is read for a numerical parameter AIMMS can translate this value to ZERO depending on the value of this option. Possible values are:



*	Never (do not translate)
*	Default_0_only (only translate when the default of the parameter involved is equal to 0)
*	Always (translate the 0 to zero for all real valued parameters)



