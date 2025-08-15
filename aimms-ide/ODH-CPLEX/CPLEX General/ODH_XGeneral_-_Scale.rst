.. _ODH-CPLEX_XGeneral_-_Scale:


Scale
=====



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Standard	



This option influences the scaling of the problem matrix. The default implements an equilibration scaling method, which is generally very effective. The "Aggressive" setting invokes a modified scaling method that can produce improvements on some problems. The setting "None" indicates that no scaling is to be done. Possible values are:



*	None (no scaling)
*	Standard (use equilibration scaling)
*	Aggressive (use aggressive scaling)



