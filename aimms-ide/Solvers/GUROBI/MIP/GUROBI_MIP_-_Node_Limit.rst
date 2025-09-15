.. _option-GUROBI-node_limit:


Node Limit
==========



:Type:	Floating point number	
:Range:	[0,1e100]	
:Default:	1e100	



This option limits the maximum number of nodes explored before the algorithm terminates without reaching optimality. For MIP usage only.


**Note** 

*	This option can be modified from within a callback within Gurobi (version 12.0 or higher) using the procedure :any:`GMP::SolverSession::SetOptionValue`.

