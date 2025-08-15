.. _KNITRO_IP_-_Linear_System_Memory_Usage:


Linear System Memory Usage
==========================



**Type**:	Selection	

**Range**:	The settings listed below	

**Default**:	Automatic	



This option indicates how to store in memory the linear systems used inside the Interior/Direct algorithm for computing primal-dual steps. Possible values are:



*	Automatic
*	Not used
*	Low
*	Normal




The 'Low' setting uses one storage location for multiple linear systems. As a result it may use much less memory, but also may be less efficient when the Interior/Direct algorithm takes a lot of CG steps. The 'Normal' setting uses separate storage for different linear systems.

