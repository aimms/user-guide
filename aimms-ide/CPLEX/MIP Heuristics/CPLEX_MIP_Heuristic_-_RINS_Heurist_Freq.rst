.. _CPLEX_MIP_Heuristic_-_RINS_Heurist_Freq:


RINS Heuristic Frequency
========================



**Type** :	Integer	

**Range** :	{-1 .. 2147483647}	

**Default** :	0	



The option determines how often to apply the relaxation induced neighborhood search heuristic (RINS heuristic). Setting the value to -1 turns off the RINS heuristic. Setting the value to 0, the default, applies the RINS heuristic at an interval chosen automatically by CPLEX. Setting the value to a positive number applies the RINS heuristic at the requested node interval. For example, setting the value to 20 dictates that the RINS heuristic be called at node 0, 20, 40, 60, etc.



