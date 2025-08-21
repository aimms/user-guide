

.. _option-IPOPT-execute_mehrotra_algorithm:


Execute Mehrotra algorithm
==========================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	No	



This option indicates if we want to do Mehrotra's algorithm. Possible values are:



*	No (do the usual IPOPT algorithm)
*	Yes (do Mehrotra's predictor-corrector algorithm)




If set to yes, IPOPT runs as Mehrotra's predictor-corrector algorithm. This works usually very well for LPs and convex QPs. This automatically disables the line search, and chooses the (unglobalized) adaptive barrier parameter strategy with the "probing" oracle (see option **Adaptive Strategy Oracle** ), and sets option **Corrector Steps Type**  to 'affine' without any safeguards; you should not set any of those options explicitly in addition.





Also, unless otherwise specified, the values of the options **Slack to Bound Minimum Absolute Distance** , **Slack to Bound Minimum Relative Distance** , and **Initial Value for Bound Multipliers**  are set more aggressive, and option **Equality Multipliers Switch Tolerance**  is set to the same value as that of the latter option.



**Learn more about** 

*	:ref:`option-IPOPT-adaptive_strategy_oracle` 
*	:ref:`option-IPOPT-corrector_steps_type` 
*	:ref:`option-IPOPT-equality_multipliers_switch_tolerance` 
*	:ref:`option-IPOPT-initial_value_for_bound_multipliers` 
*	:ref:`option-IPOPT-point_to_bound_absolute_distance` 
*	:ref:`option-IPOPT-point_to_bound_relative_distance` 
