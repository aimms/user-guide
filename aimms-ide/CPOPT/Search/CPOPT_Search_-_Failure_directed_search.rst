.. _option-CPOPT-failure_directed_search:


Failure directed search
=======================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	On	



This option controls usage of failure-directed search. Possible values are:



*	Off
*	On




Failure-directed search assumes that there is no (better) solution or that such a solution is very hard to find. Therefore it focuses on systematic exploration of the search space, first eliminating assignments that are most likely to fail. Failure-directed search is used only for scheduling problems (i.e. models containing activities) and only when the option **Search Type**  is set to 'Restart' or 'Automatic'.





When this option is switched on then CP Optimizer starts failure-directed search when other search strategies are (no longer) successful and when the memory necessary for the search does not exceed the value set by the option **Failure Directed Search Memory Limit** .





**Learn more about** 

*	:ref:`option-CPOPT-failure_directed_search_emphasis` 
*	:ref:`option-CPOPT-failure_directed_search_memory_limit` 
*	:ref:`option-CPOPT-search_type` 
