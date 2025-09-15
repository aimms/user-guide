.. _option-GUROBI-soft_memory_limit:


Soft Memory Limit
=================



:Type:	Floating point number	
:Range:	[0,1e100]	
:Default:	1e100



This option limits the total amount of memory (in GB, i.e., :math:`10^9` bytes) available to Gurobi. If more is needed, Gurobi will fail
with an out-of-memory error.

In contrast to the **Memory Limit** option, is option leads to a graceful exit of the optimization, such that it is possible to retrieve 
solution information afterwards or (in the case of a MIP solve) resume the optimization.

A disadvantage compared to **Memory Limit** is that this option is only checked at places where optimization can be terminated gracefully,
so memory use may exceed the limit between these checks.

Memory usage is tracked across all threads. One consequence of this is that termination may be non-deterministic for multi-threaded runs.


**Learn more about** 

*	:ref:`option-GUROBI-memory_limit`  

