.. _SNOPT_SQP_-_DifferenceInterval:


Difference Interval
===================



:Type:	Floating point number	
:Range:	[0,1] + {na}	
:Default:	na	



This option alters the interval h1 that is used to estimate gradients by forward differences in the following circumstances: 


*   In the initial ("cheap") phase of verifying the objective gradients. 
*   For verifying the constraint gradients. 
*   For estimating missing objective gradients. 
*   For estimating missing Jacobian elements.



In the last three cases, a derivative with respect to xj is estimated by perturbing that 
component of x to the value :math:`xj + h1(1 +| xj |)`, and then evaluating F(x) or f(x) at the perturbed point. 
The resulting gradient estimates should be accurate to O(h1) unless the functions are badly scaled. 
Judicious alteration of h1 may sometimes lead to greater accuracy.



The default value of this option depends on the relative precision of the computer being used. On most computers the default equals 1.5e-8.



**Learn more about** 

*	:ref:`SNOPT_SQP_-_DerivativeOption`  
