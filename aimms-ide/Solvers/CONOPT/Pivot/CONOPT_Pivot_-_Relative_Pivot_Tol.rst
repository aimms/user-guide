.. _option-CONOPT-relative_pivot_tolerance:

Relative Pivot Tolerance
========================



:Type:	Floating point number	
:Range:	[0.001,0.9]	
:Default:	0.05	



A pivot element is only considered acceptable relative to other elements in the column if its absolute value is at least the value of this option times the largest absolute value in the column. You may have to increase this value towards 1.0 with poorly scaled models. Increasing the value of this option will result in denser L and U factors of the basis.



**Learn more about** 

*	:ref:`option-CONOPT-absolute_pivot_tolerance_nonlinear_elements`  
