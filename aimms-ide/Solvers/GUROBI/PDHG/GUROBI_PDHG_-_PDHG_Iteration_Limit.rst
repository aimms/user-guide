.. _option-GUROBI-pdhg_iteration_limit:


PDHG Iteration Limit
====================



:Type:	Floating point number	
:Range:	[0.0,1e100]	
:Default:	1e100	



This option limits the number of PDHG iterations performed.

The PDHG algorithm will terminate if this limit is exceeded. If crossover is enabled, it will start from the final PDHG iterate.


**Note** 

*	This option was added in Gurobi 13.0.

