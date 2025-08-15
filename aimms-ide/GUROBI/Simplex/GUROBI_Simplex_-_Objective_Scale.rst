.. _GUROBI_Simplex_-_Objective_Scale:


Objective Scale
===============



:Type:	Floating point number	
:Range:	[-1,1e100]	
:Default:	0



The model objective is divided by the specified value of this option to avoid numerical errors that may result from very large objective coefficients. The default value of 0 decides on the scaling automatically. A value less than zero uses the maximum coefficient to the specified power as the scaling (so a value of -0.5 would scale by the square root of the largest objective coefficient).

