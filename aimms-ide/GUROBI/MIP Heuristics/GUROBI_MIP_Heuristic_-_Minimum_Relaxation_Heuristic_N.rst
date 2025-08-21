.. _option-GUROBI-minimum_relaxation_heuristic_node_limit:


Minimum Relaxation Heuristic Node Limit
=======================================



:Type:	Integer	
:Range:	{-1 .. 2000000000}	
:Default:	-1	



This option specifies the number of nodes to explore in the Minimum Relaxation heuristic. The default value of -1 chooses automatically. Note that this heuristic is only applied at the end of the MIP root, and only when no other root heuristic finds a feasible solution.

