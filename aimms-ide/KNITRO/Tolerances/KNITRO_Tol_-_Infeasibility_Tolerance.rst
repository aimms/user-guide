.. _KNITRO_Tol_-_Infeasibility_Tolerance:


Infeasibility Tolerance
=======================



:Type:	Floating point number	
:Range:	[0,1e20]	
:Default:	1e-8	



This option specifies the (relative) tolerance used for declaring infeasibility of a model. Smaller values of this option make it more difficult to satisfy the conditions Knitro uses for detecting infeasible models. If you believe Knitro incorrectly declares a model to be infeasible, then you should try a smaller value for this option.



**Learn more about** 

*	:ref:`KNITRO_Term_-_Infeas_Tol_Iteration_Limit` 
