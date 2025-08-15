.. _KNITRO_IP_-_Barrier_Switch_Rule:


Barrier Switch Rule
===================



**Type**:	Selection	

**Range**:	The settings listed below	

**Default**:	Automatic	



This option indicates whether or not the barrier algorithms will allow switching from an optimality phase to a pure feasibility phase. Possible values are:



*	Automatic
*	Off
*	Normal
*	Aggressive




With setting 'Off' Knitro never switches to the feasibility phase. With setting 'Normal' Knitro allows switches to the feasibility phase and with setting 'Aggressive' a more aggressive switching rule is used.





This option has no effect on the Active Set and SQP algorithms.





**Learn more about** 

*	:ref:`KNITRO_General_-_Algorithm` 
