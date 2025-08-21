.. _option-CPLEX-stalled_iterations:


Stalled Iterations
==================



:Type:	Integer	
:Range:	{0 .. 2100000000}	
:Default:	0	



The primal and dual simplex methods include a perturbation mechanism for dealing with situations in which no progress has been made in the objective function over a significant number of iterations. This phenomenon is sometimes called stalling. With default settings (value 0), the number of stalled iterations before perturbation is invoked is determined internally by CPLEX depending upon problem dimensions. However, when the user sets this option to a positive value, that value becomes the limit on stalled iterations before perturbation will be performed.



