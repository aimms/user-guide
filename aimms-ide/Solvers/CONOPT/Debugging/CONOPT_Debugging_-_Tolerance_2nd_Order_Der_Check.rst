.. _option-CONOPT-tolerance_2nd_order_derivatives_check:

Tolerance 2nd Order Derivatives Check
=====================================



:Type:	Floating point number	
:Range:	[0.0,1.0]	
:Default:	6e-7	



The second order derivatives calculated by AIMMS are tested by CONOPT if the option **Check 2nd Order Derivatives** is activated. If the difference between a second order derivative calculated by AIMMS and the estimation by CONOPT is larger than the value of this option, then the second order derivative calculated by AIMMS is considered to be incorrect, and an error message is issued.



**Learn more about** 

*	:ref:`option-CONOPT-check_2nd_order_derivatives`  



