

.. _option-IPOPT-adaptive_strategy_factor_limit:


Adaptive strategy factor limit
==============================



:Type:	Floating point number	
:Range:	[0,1e+019]	
:Default:	1000	



This option specifies the factor for initialization of maximum value for the barrier parameter. It determines the upper bound on the barrier parameter. This upper bound is computed as the average complementarity at the initial point times the value of this option.



**Note** 

*	This option is only used if the setting of option **Barrier Parameter Update Strategy**  equals 'Adaptive'.




**Learn more about** 

*	:ref:`option-IPOPT-barrier_parameter_update_strategy` 
