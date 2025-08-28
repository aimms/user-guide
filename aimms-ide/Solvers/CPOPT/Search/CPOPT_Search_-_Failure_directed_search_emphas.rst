.. _option-CPOPT-failure_directed_search_emphasis:


Failure directed search emphasis
================================



:Type:	Floating point number	
:Range:	[-1,1e10]	
:Default:	-1	



This option specifies how much time CP Optimizer will invest in failure-directed search. The default value of -1 has a special meaning. At this setting, CP Optimizer observes the actual performance of failure-directed search and decides automatically how much time is invested.



Any other value means that once failure-directed search has started, it is used by the given number of workers. The value does not have to be integer. For example, value 1.5 means that the first worker spends 100% of the time by failure-directed search, the second worker 50% and remaining workers 0%. 



**Learn more about** 

*	:ref:`option-CPOPT-failure_directed_search` 
*	:ref:`option-CPOPT-number_of_workers` 
