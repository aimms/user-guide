.. _option-CONOPT-feasibility_tolerance_triangular_part:

Feasibility Tolerance Triangular Part
=====================================



:Type:	Floating point number	
:Range:	[3e-13,1e-4]
:Default:	1e-8



Triangular equations are usually solved to an accuracy of **Minimal Feasibility Tolerance** . However, if a variable reaches a bound or if a constraint only has pre-determined variables then the feasibility tolerance can be relaxed to the value of this option.



**Learn more about** 

*	:ref:`option-CONOPT-minimal_feasibility_tolerance`  



