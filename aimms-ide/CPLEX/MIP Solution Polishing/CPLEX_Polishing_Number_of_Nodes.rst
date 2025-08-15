.. _CPLEX_Polishing_Number_of_Nodes:


Polishing Number of Nodes
=========================



**Type**:	Integer	

**Range**:	{0 .. 2147483647}	

**Default**:	2147483647	



This option sets the number of nodes processed in branch-and-cut before CPLEX starts solution polishing, if a feasible solution is available. When this parameter is set to 0, CPLEX completes processing at the root; that is, it creates cuts and applies heuristics at the root. When this parameter is set to 1 (one), it allows branching from the root; that is, nodes are created but not solved. When no feasible solution is available yet, CPLEX explores more nodes than the number specified by this parameter.



CPLEX must have a feasible solution in order to start polishing. It must also have certain internal structures in place to support solution polishing. Consequently, when the criterion specified by this parameter is met, CPLEX begins solution polishing only after these starting conditions are also met. That is, there may be a delay between the moment when the criterion specified by this parameter is met and when solution polishing starts.



