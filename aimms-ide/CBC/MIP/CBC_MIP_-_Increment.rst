.. _CBC_-_Increment:


Increment
=========



:Type:	Floating point number	
:Range:	[-1e20,1e20]	
:Default:	1e-5	



A valid solution must be at least this much better than the last integer solution. Whenever a solution is found for a MIP problem, the bound on solutions is set to solution (in a minimization sense) plus the value of this option. If it is not set then CBC will try and work one out, e.g., if all objective coefficients are multiples of 0.01 and only integer variables have entries in the objective then this can be set to 0.01. Be careful if you set this option to a negative value.

