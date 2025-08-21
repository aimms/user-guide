.. _option-CONOPT-zero_filter_tolerance_jacobian_elements:

Zero Filter Tolerance Jacobian Elements
=======================================



:Type:	Floating point number	
:Range:	[1e-30,1]
:Default:	1e-20	



This option specifies the zero filter for Jacobian elements and inversion results. It determines the smallest absolute value that an intermediate result can have. If it is smaller, it is set to 0 (zero). It must be smaller than **Absolute Pivot Tolerance**  / 10.



**Learn more about** 

*	:ref:`option-CONOPT-absolute_pivot_tolerance` 
