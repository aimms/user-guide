.. _option-GUROBI-barrier_iteration_limit:


Barrier Iteration Limit
=======================



:Type:	Integer	
:Range:	{0 .. 2000000000}	
:Default:	1000	



This option limits the number of barrier iterations performed.


**Note** 

*	This option can be modified from within a callback within Gurobi (version 12.0 or higher) using the procedure :any:`GMP::SolverSession::SetOptionValue`.

