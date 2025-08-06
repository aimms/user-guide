.. _CBC_Barrier_-_Barrier_crossover:


Barrier crossover
=================



**Type** :	Selection	

**Range** :	The settings listed below	

**Default** :	On	



This option determines whether to get a basic solution after using the barrier algorithm. Possible values are:



*	Off
*	On




Interior point algorithms do not obtain a basic solution (and the feasibility criterion is a bit suspect). This option will crossover to a basic solution suitable for ranging or branch and cut.




