.. _option-CPOPT-cardinality_encoding:


Cardinality encoding
====================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Count	



This option determines the encoding used for Cardinality constraints. Possible values are:



*	Count
*	Distribute




With setting 'Count' the AIMMS-CP Optimizer interface uses the IloCount function of CP Optimizer and with setting 'Distribute' it uses the IloDistribute class.

