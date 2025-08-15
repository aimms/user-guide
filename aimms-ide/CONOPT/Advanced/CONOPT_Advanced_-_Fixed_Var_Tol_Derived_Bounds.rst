.. _CONOPT_Advanced_-_Fixed_Var_Tol_Derived_Bounds:

Fixed Variables Tolerance Derived Bounds
========================================



:Type:	Floating point number	
:Range:	[3e-13,1e-8]
:Default:	1e-12	



A variable is considered fixed if the distance between the bounds is less than FVT * Max(1,Abs(Bound)), where FVT denotes the value of this option. The tolerance is used both on the users original bounds and on the derived bounds that the preprocessor implies from the constraints of the model.



**Learn more about** 

*	:ref:`CONOPT_General_-_Bound_Tolerance` 
