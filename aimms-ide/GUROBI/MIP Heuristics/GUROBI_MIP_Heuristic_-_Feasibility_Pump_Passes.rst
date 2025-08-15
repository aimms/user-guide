.. _GUROBI_MIP_Heuristic_-_Feasibility_Pump_Passes:


Feasibility Pump Passes
=======================



:Type:	Integer	
:Range:	{-1 .. 2000000000}	
:Default:	-1	



This option sets the number of passes of the feasibility pump heuristic. Note that this heuristic is only applied at the end of the MIP root, and only when no other root heuristic found a feasible solution.



This heuristic is quite expensive, and generally produces poor quality solutions. You should generally only use it if other means, including exploration of the tree with default settings, fail to produce a feasible solution.



