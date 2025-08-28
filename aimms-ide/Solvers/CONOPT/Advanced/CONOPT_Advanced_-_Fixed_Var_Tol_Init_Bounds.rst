.. _option-CONOPT-fixed_variables_tolerance_initial_bounds:

Fixed Variables Tolerance Initial Bounds
========================================



:Type:	Floating point number	
:Range:	[3e-13,1e-5]
:Default:	1e-9	



This option specifies the tolerance for defining variables as fixed based on initial bounds. A variable is considered fixed if the distance between the bounds defined by the user is less than FVT * Max(1,Abs(Bound)), where FVT denotes the value of this option.



**Learn more about** 

*	:ref:`option-CONOPT-bound_tolerance` 
