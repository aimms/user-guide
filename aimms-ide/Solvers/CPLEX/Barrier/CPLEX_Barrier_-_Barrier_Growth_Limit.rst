.. _option-CPLEX-barrier_growth_limit:


Barrier Growth Limit
====================



:Type:	Floating point number	
:Range:	[1, inf)	
:Default:	1e12	



This option is used to detect unbounded optimal faces. At higher values, the barrier algorithm will be less likely to conclude that the problem has an unbounded optimal face, but more likely to have numerical difficulties if the problem has an unbounded face.



