.. _option-KNITRO-absolute_feasibility_tolerance:


Absolute Feasibility Tolerance
==============================



:Type:	Floating point number	
:Range:	[0,1e20]	
:Default:	0.001	



This option specifies the final absolute stopping tolerance for the feasibility error. Smaller values for this option result in a higher degree of accuracy in the solution with respect to feasibility.



The feasibility error is defined as the maximum violation among all constraints. It is 0 if there are no constraint violations.



**Learn more about** 

*	:ref:`option-KNITRO-relative_feasibility_tolerance`  
