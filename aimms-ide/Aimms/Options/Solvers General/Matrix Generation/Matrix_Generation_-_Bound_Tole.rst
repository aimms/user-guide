

.. _Options_Matrix_Generation_-_Bound_Tole:


Bound Tolerance
===============



:Type:	Floating point number	
:Range:	[0,1]	
:Default:	1e-8	



The Bound Tolerance option is used for variable marking and error messages on the feasibility of variables and constraints. If the level value of a variable exceeds its bounds by more than Bound Tolerance, then that variable is marked in the solution listing. If during the generation of a model, the lower bound is above the upper bound by more than Bound Tolerance, an error message is issued. In addition, if during generation of a constraint it is infeasible by more than Bound Tolerance, an error message is issued.



This option also affects variables that are fixed using the .Nonvar suffix, using a value of 1, but only if the level value of the variable is outside its bounds. If the bound violation is greater than the bound tolerance then the level value will be rounded to the nearest bound, and otherwise not. For example, assume X is a nonnegative variable. If we use



	X := -1e-6;

	X.Nonvar := 1.



then X will be fixed to 0 if the bound tolerance is at its default setting of 1e-8, and X will be fixed to -1e-6 if we change the bound tolerance to 1e-5.

