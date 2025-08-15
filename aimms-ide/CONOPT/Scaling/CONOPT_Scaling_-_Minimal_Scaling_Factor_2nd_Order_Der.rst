.. _CONOPT_Scaling_-_Minimal_Scaling_Factor_2nd_Order_Der:

Minimal Scaling Factor 2nd Order Derivatives
============================================



:Type:	Floating point number	
:Range:	[1e-9,1.0]	
:Default:	1e-6	



This option sets a lower bound for scale factors based on large 2nd derivatives. Scaling of the model is in most cases based on the values of the variables and the first derivatives. However, if the scaled variables and derivatives are reasonable but there are large values in the Hessian of the Lagrangian (the matrix of 2nd derivatives) then the lower bound on the scale factor can be made smaller than the **Minimal Scaling Factor** . CONOPT will try to scale variables with large 2nd order derivatives by one over the square root of the diagonal elements of the Hessian. However, the revised scale factors cannot be less than the value of this option.



**Learn more about** 

*	:ref:`CONOPT_Scaling_-_Minimal_Scaling_Factor`  
