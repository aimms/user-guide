

.. _IPOPT_Barrier_-_Superlinear_decrease_rate_barrier_parameter:


Superlinear decrease rate barrier parameter
===========================================



**Type**:	Floating point number	

**Range**:	[1,2]	

**Default**:	1.5	



This option determines the superlinear decrease rate of the barrier parameter. For the Fiacco-McCormick update procedure the new barrier parameter (mu) is obtained by taking the minimum of mu*v and w, where v denotes the value of the option **Linear Decrease Factor Barrier Parameter**  and w denotes the value of this option.



This option is also used in the adaptive barrier parameter strategy during the monotone mode.



**Learn more about** 

*	:ref:`IPOPT_Barrier_-_Barrier_parameter_update_strategy` 
*	:ref:`IPOPT_Barrier_-_Linear_decrease_factor_barrier_parameter` 
