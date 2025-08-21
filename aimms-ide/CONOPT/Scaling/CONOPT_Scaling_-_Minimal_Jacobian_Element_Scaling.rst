.. _option-CONOPT-minimal_jacobian_element_for_scaling:

Minimal Jacobian Element for Scaling
====================================



:Type:	Floating point number	
:Range:	[1e-7,0.001]	
:Default:	1e-5	



This option is to avoid problems with zero and very small Jacobian elements; all elements with a value less than the value of this option are rounded up to the value of this option.



