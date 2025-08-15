.. _GUROBI_Simplex_-_Degenerate_Simplex_Moves_Limit:


Degenerate Simplex Moves Limit
==============================



:Type:	Integer	
:Range:	{-1 .. 2000000000}	
:Default:	-1	



This option limits degenerate simplex moves. These moves are performed to improve the integrality of the current relaxation solution. By default, the algorithm chooses the number of moves to perform automatically.



Changing the value of this option can help performance in cases where an excessive amount of time is spent after the initial root relaxation has been solved but before the cut generation process or the root heuristics have started.



**Note** 

*	This option only affects mixed integer programming (MIP) models.



