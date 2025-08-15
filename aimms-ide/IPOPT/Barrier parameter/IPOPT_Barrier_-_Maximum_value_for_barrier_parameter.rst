

.. _IPOPT_Barrier_-_Maximum_value_for_barrier_parameter:


Maximum value for barrier parameter
===================================



:Type:	Floating point number	
:Range:	[0,1e+019]	
:Default:	100000	



This option specifies an upper bound on the barrier parameter in the adaptive barrier parameter selection mode. If this option is set, it overwrites the effect of option **Adaptive Strategy Factor Limit** .



This option is only used if 'Adaptive' is selected for option **Barrier Parameter Update Strategy** .



**Learn more about** 

*	:ref:`IPOPT_Barrier_-_Adaptive_strategy_factor_limit` 
*	:ref:`IPOPT_Barrier_-_Barrier_parameter_update_strategy` 
