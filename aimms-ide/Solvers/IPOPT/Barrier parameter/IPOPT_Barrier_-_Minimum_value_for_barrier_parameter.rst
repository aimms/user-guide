

.. _option-IPOPT-minimum_value_for_barrier_parameter:


Minimum value for barrier parameter
===================================



:Type:	Floating point number	
:Range:	[0,1e+019]	
:Default:	1e-011	



This option specifies the lower bound on the barrier parameter in the adaptive barrier parameter selection mode. By default, it is set to the minimum of 1e-11 and min(u,v)/(w+1), which should be a reasonable value. Here:



u is the value of the option **Relative Convergence Tolerance** ,

v is the value of the option **Complementarity Tolerance** , and

w is the value of the option **Barrier Convergence Tolerance Factor** .



This option is only used if 'Adaptive' is selected for option **Barrier Parameter Update Strategy** .



**Learn more about** 

*	:ref:`option-IPOPT-barrier_convergence_tolerance_factor` 
*	:ref:`option-IPOPT-barrier_parameter_update_strategy` 
*	:ref:`option-IPOPT-complementarity_tolerance` 
*	:ref:`option-IPOPT-relative_convergence_tolerance` 



