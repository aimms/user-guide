.. _GUROBI_MIP_Heuristic_-_Zero_Objective_Node_Limit:


Zero Objective Node Limit
=========================



**Type** :	Integer	

**Range** :	{-1 .. 2000000000}	

**Default** :	-1	



This option limits the number of nodes to explore in the zero objective heuristic. Note that this heuristic is only applied at the end of the MIP root, and only when no other root heuristic finds a feasible solution.



This heuristic is quite expensive, and generally produces poor quality solutions. You should generally only use it if other means, including exploration of the tree with default settings, fail to produce a feasible solution.

