.. _KNITRO_IP_-_Barrier_Penalty_Parameter_St:


Barrier Penalty Parameter Strategy
==================================



**Type** :	Selection	

**Range** :	The settings listed below	

**Default** :	Automatic	



This option indicates which penalty parameter strategy to use for determining whether or not to accept a trial iterate. Possible values are:



*	Automatic
*	Single parameter
*	Multiple parameters




With setting 'Single parameter' Knitro uses a single penalty parameter in the merit function to weight feasibility versus optimality. With setting 'Multiple parameters' Knitro uses a more tolerant and flexible step acceptance procedure based on a range of penalty parameter values. This setting can often accelerate convergence.





This option has no effect on the Active Set and SQP algorithms.





**Learn more about** 

*	:ref:`KNITRO_General_-_Algorithm` 
