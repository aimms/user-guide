.. _GUROBI_Parallel_-_Thread_Limit:


Thread Limit
============



:Type:	Integer	
:Range:	{0 .. 2000000000}	
:Default:	0	



This option controls the number of threads to apply to parallel algorithms (parallel MIP, concurrent MIP, concurrent LP and parallel barrier). The default value of 0 is an automatic setting. It will generally use as many threads as there are virtual processors. The number of virtual processors may exceed the number of cores due to hyperthreading or other similar hardware features.



While you will generally get the best performance by using all available cores in your machine, there are a few exceptions. One is of course when you are sharing a machine with other jobs. In this case, you should select a thread count that doesn't oversubscribe the machine.



Certain classes of MIP models benefit from reducing the thread count, often all the way down to one thread. Starting multiple threads introduces contention for machine resources. For classes of models where the first solution found by the MIP solver is almost always optimal, and that solution isn't found at the root, it is often better to allow a single thread to explore the search tree uncontested.



Another situation where reducing the thread count can be helpful is when memory is tight. Each thread can consume a significant amount of memory.



Gurobi imposes a soft limit of 32 threads for the automatic setting (0). If your machine has more, and you find that using more increases performance, you should feel free to set this option to a larger value.



**Note** 

*	The algorithms for parallel MIP, parallel barrier and concurrent LP, if the option **Method**  is set to 'Deterministic concurrent', are deterministic which means that multiple runs with the same model at the same option settings on the same platform will reproduce the same solution path and results.
*	This option also limits the number of threads used by the **Concurrent MIP**  solver.




**Learn more about** 

*	:ref:`GUROBI_Parallel_-_Concurrent_MIP` 
*	:ref:`GUROBI_General_-_Method` 



