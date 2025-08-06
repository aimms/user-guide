.. _ODH-CPLEX_XMIP_-_Max_Nr_of_Nodes:


Maximal Number of Nodes
=======================



**Type** :	Integer	

**Range** :	{0 .. 2147483647}	

**Default** :	2147483647	



This option sets the maximum number of nodes solved before the algorithm terminates without reaching optimality. When this option is set to 0, CPLEX completes processing at the root; that is, it creates cuts and applies heuristics at the root. When this option is set to 1, it allows branching from the root; that is, nodes are created but not solved.



