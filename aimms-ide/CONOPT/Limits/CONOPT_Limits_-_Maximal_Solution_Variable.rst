.. _option-CONOPT-maximum_solution_of_a_variable:

Maximum Solution of a Variable
==============================



:Type:	Floating point number	
:Range:	[1e+5,1e+30]
:Default:	1e15	



If the value of a variable, including the objective function value and the value of slack variables, exceeds the value of this option, then the model is considered to be unbounded and the optimization process is stopped.



If you need a larger value, then your model is probably poorly scaled and CONOPT may have difficulties solving it.



