

.. _IPOPT_Barrier_-_Fixed_mode_oracle:


Fixed mode oracle
=================



**Type** :	Selection	

**Range** :	The settings listed below	

**Default** :	Average complementarity	



This option sets the oracle for the barrier parameter when switching to fixed mode. It determines how the first value of the barrier parameter should be computed when switching to the "monotone mode" in the adaptive strategy. It is only considered if 'Adaptive' is selected for option **Barrier Parameter Update Strategy** . Possible values are:



*	Probing
*	Loqo
*	Quality function
*	Average complementarity




Setting 'probing' corresponds to Mehrotra's probing heuristic. Setting 'Loqo' refers to LOQO's centrality rule.





**Learn more about** 

*	:ref:`IPOPT_Barrier_-_Barrier_parameter_update_strategy` 
