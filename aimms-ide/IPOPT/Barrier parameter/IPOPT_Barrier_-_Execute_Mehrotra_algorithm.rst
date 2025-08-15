

.. _IPOPT_Barrier_-_Execute_Mehrotra_algorithm:


Execute Mehrotra algorithm
==========================



**Type**:	Selection	

**Range**:	The settings listed below	

**Default**:	No	



This option indicates if we want to do Mehrotra's algorithm. Possible values are:



*	No (do the usual IPOPT algorithm)
*	Yes (do Mehrotra's predictor-corrector algorithm)




If set to yes, IPOPT runs as Mehrotra's predictor-corrector algorithm. This works usually very well for LPs and convex QPs. This automatically disables the line search, and chooses the (unglobalized) adaptive barrier parameter strategy with the "probing" oracle (see option **Adaptive Strategy Oracle** ), and sets option **Corrector Steps Type**  to 'affine' without any safeguards; you should not set any of those options explicitly in addition.





Also, unless otherwise specified, the values of the options **Slack to Bound Minimum Absolute Distance** , **Slack to Bound Minimum Relative Distance** , and **Initial Value for Bound Multipliers**  are set more aggressive, and option **Equality Multipliers Switch Tolerance**  is set to the same value as that of the latter option.



**Learn more about** 

*	:ref:`IPOPT_Barrier_-_Adaptive_strategy_oracle` 
*	:ref:`IPOPT_Line_search_-_Corrector_steps_type` 
*	:ref:`IPOPT_Multipliers_-_Equality_multipliers_switch_tolerance` 
*	:ref:`IPOPT_Initialization_-_Initial_value_for_bound_multipliers` 
*	:ref:`IPOPT_Initialization_-_Point_to_bound_absolute_distance` 
*	:ref:`IPOPT_Initialization_-_Point_to_bound_relative_distance` 
