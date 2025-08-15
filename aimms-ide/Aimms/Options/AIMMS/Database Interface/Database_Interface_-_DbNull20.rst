

.. _Options_Database_Interface_-_DbNull20:


Database Translate Null to 0
============================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Off	



A NULL in databases can be interpreted as a default of the parameter or as an explicit 0. When this option is set to on and the default of the parameter is not equal to 0 then AIMMS translates a NULL to 0 for real valued parameters. Possible values are:



*	On 
*	Off 



