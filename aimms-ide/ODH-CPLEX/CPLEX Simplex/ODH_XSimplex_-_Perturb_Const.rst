.. _ODH-CPLEX_XSimplex_-_Perturb_Const:


Perturbation Constant
=====================



:Type:	Floating point number	
:Range:	[1e-8,INF]	
:Default:	1e-6	



The amount by which CPLEX will perturb the upper and lower bounds on the variables when a problem is perturbed can be set using this option. It can be set to a smaller value if the default value creates too large a change in the problem.



