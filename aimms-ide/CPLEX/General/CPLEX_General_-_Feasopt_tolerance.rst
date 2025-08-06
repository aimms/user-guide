.. _CPLEX_General_-_Feasopt_tolerance:


Feasopt Tolerance
=================

**Type** :	Floating point number	

**Range** :	[0,inf)	

**Default** :	1e-6	



This option controls the amount of relaxation for FeasOpt (Feasibility Relaxation).


In the case of a Mixed Integer Program, this option specifies the absolute gap for computing the minimum-cost relaxation in Phase I. 



In the case of a Linear Program, this option controls the lower objective limit when computing the minimum-cost relaxation in Phase I. Therefore, it is only relevant if the primal optimizer is being used. 



Using this option, you can implement other stopping criteria as well. To do so, first run FeasOpt with the stopping criteria that you prefer; then set this parameter to the resulting objective of the minimum-cost relaxation returned by Phase I; unset the other stopping criteria, and run FeasOpt again. Since the solution from the first call already matches this parameter, Phase I will terminate immediately in this second call to FeasOpt, and Phase II will start.



**Learn more about** 

· 	:ref:`CPLEX_Feasibility_Relaxation`  

