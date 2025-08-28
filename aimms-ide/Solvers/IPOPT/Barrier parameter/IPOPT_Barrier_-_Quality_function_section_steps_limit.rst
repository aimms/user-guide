

.. _option-IPOPT-quality_function_section_steps_limit:


Quality function section steps limit
====================================



:Type:	Integer	
:Range:	{0..2147483647}	
:Default:	8	



This option specifies the maximum number of search steps during the direct search procedure determining the optimal centering parameter. The golden section search is performed for the quality function based barrier parameter oracle.



This option is only used if 'Quality function' is selected for option **Adaptive Strategy Oracle**.



**Learn more about** 

*	:ref:`option-IPOPT-adaptive_strategy_oracle` 
