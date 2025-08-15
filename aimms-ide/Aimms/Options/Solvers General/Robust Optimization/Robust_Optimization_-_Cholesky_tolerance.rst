

.. _Options_Robust_Optimization_-_Cholesky_tolerance:


Cholesky Tolerance
==================



:Type:	Floating point number	
:Range:	[0,1]	
:Default:	1e-8	



To create the robust counterpart of a linear model with ellipsoidal uncertainty, Cholesky decomposition is done on quadratic matrices. Diagonal elements in the quadratic matrix are considered as 0 if their absolute value is smaller than or equal to the value of this option.

