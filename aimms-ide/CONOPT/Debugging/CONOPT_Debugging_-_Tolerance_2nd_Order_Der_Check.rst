.. _CONOPT_Debugging_-_Tolerance_2nd_Order_Der_Check:

Tolerance 2nd Order Derivatives Check
=====================================



**Type** :	Floating point number	

**Range** :	[0.0,1.0]	

**Default** :	6e-7	



The second order derivatives calculated by AIMMS are tested by CONOPT if the option **Check 2nd Order Derivatives** is activated. If the difference between a second order derivative calculated by AIMMS and the estimation by CONOPT is larger than the value of this option, then the second order derivative calculated by AIMMS is considered to be incorrect, and an error message is issued.



**Learn more about** 

*	:ref:`CONOPT_Debugging_-_Check_2nd_Order_Der`  



