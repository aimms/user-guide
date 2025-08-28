.. _option-CONOPT-absolute_pivot_tolerance_nonlinear_elements:

Absolute Pivot Tolerance Nonlinear Elements
===========================================



:Type:	Floating point number	
:Range:	[2.2e-16,0.001]	
:Default:	1e-5	



This option specifies the smallest pivot that can be used for nonlinear or variable Jacobian elements during the pre-triangular solve. The pivot tolerance for linear or constant Jacobian elements is determined by the option **Absolute Pivot Tolerance**. The value of this option cannot be less than the **Absolute Pivot Tolerance**.



**Learn more about** 

*	:ref:`option-CONOPT-absolute_pivot_tolerance_nonlinear_elements`  
