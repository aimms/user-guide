.. _CPOPT_Search_-_Failure_directed_search_memory:


Failure directed search memory limit
====================================



**Type**:	Integer	

**Range**:	{0..2100000000}	

**Default**:	104857600



This option controls the maximum amount of memory (in bytes) available to failure-directed search. The default corresponds to 100MB.



Failure-directed search can sometimes consume a lot of memory, especially when end times of interval variables are not bounded. Therefore it is usually not started immediately, but only when the effective horizon (time period over which CP Optimizer must reason) becomes small enough for failure-directed search to operate inside the memory limit specified by this option. For many types of scheduling problems, the effective horizon tends to reduce when CP Optimizer finds a better solution (often most significantly when the initial solution is found). Therefore, when each new solution is found, CP Optimizer decides whether or not to turn on failure-directed search.



**Note** 

*	This option does not influence the effectiveness of failure-directed search, once started. Its purpose is only to control the point at which failure-directed search will begin to function




**Learn more about** 

*	:ref:`CPOPT_Search_-_Failure_directed_search` 






