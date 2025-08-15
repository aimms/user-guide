

.. _IPOPT_Barrier_-_Adaptive_strategy_oracle:


Adaptive strategy oracle
========================



**Type**:	Selection	

**Range**:	The settings listed below	

**Default**:	Quality function	



This option determines how a new barrier parameter is computed in each "free-mode" iteration of the adaptive barrier parameter strategy.Possible values are:



*	Probing
*	Loqo
*	Quality function




Setting 'probing' corresponds to Mehrotra's probing heuristic. Setting 'Loqo' refers to LOQO's centrality rule.





**Note** 

*	This option is only used if the setting of option **Barrier Parameter Update Strategy**  equals 'Adaptive'.




**Learn more about** 

*	:ref:`IPOPT_Barrier_-_Barrier_parameter_update_strategy` 
