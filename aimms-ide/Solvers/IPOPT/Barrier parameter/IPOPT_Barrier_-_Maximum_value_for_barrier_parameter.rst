

.. _option-IPOPT-maximum_value_for_barrier_parameter:


Maximum value for barrier parameter
===================================



:Type:	Floating point number	
:Range:	[0,1e+019]	
:Default:	100000	



This option specifies an upper bound on the barrier parameter in the adaptive barrier parameter selection mode. If this option is set, it overwrites the effect of option **Adaptive Strategy Factor Limit**.



This option is only used if 'Adaptive' is selected for option **Barrier Parameter Update Strategy**.



**Learn more about** 

*	:ref:`option-IPOPT-adaptive_strategy_factor_limit` 
*	:ref:`option-IPOPT-barrier_parameter_update_strategy` 
