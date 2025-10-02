.. _option-GUROBI-nonlinear_optimality_tolerance:


Nonlinear Optimality Tolerance
==============================



:Type:	Floating point number	
:Range:	[0.0,1e100]	
:Default:	1e-4	



This option specifies the relative optimality tolerance used for NLP and MINLP models. Gurobi will terminate (with an optimal result)
when the gap between the lower and upper objective bound is less than *z* times the absolute value of the incumbent objective value,
where *z* is the value of this option.



