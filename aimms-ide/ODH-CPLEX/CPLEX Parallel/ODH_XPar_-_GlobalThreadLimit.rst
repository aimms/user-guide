.. _option-ODHCPLEX-global_thread_limit:


Global Thread Limit
===================



:Type:	Integer	
:Range:	{0 .. 2100000000}	
:Default:	0	



This option sets the maximal number of parallel threads that will be invoked by any CPLEX parallel optimizer. This option interacts with the Parallel Mode option. CPLEX can use parallel threads for solving MIP models and, if the barrier algorithm is used, for solving LP, QP and QCP models.



For a single thread, the parallel algorithms behave deterministically, regardless of thread option settings; that is, the algorithm proceeds sequentially in a single thread.



In this context, sequential means that the algorithm proceeds step by step, consecutively, in a predictable and repeatable order within a single thread. Deterministic means that repeated solving of the same model with the same option settings on the same computing platform will follow exactly the same solution path, yielding the same level of performance and the same values in the solution. Sequential execution is deterministic. In multithreaded computing, a deterministic setting requires synchronization between threads. Opportunistic entails less synchronization between threads and thus may offer better performance at the sacrifice of repeatable, invariant solution paths and values in repeated runs on multiple threads or multiple processors.



We distinguish informational callbacks from control callbacks. The callbacks for incumbent, iterations and status change are informational callbacks. These callbacks are used to retrieve certain information from CPLEX. The callbacks for branch, candidate, cut, heuristic and lazy constraints are control callbacks. Control callbacks allow you to control the branch & cut search during the optimization of MIP problems.



When this option is at its default setting 0, and your application includes no callbacks or only informational callbacks, CPLEX can use all available threads; that is, at most 32 threads or the number of cores of the machine, whichever is smaller. If your machine offers more than 32 threads, you can take advantage of them by increasing the value of this option.



When this option is at its default setting 0, and your application includes a control callback, then CPLEX uses one thread. In other words, the presence of a control callback turns off parallel processing when the value of this option is at its default.



In order to use parallel optimization in conjunction with control callbacks, you need to set this option to a positive value. However, when you do so, you need to be aware of the fact that the callbacks may be invoked concurrently, and that the algorithm might become opportunistic even if the option **Parallel Mode**  is set to 'Deterministic'.



This option also determines the amount of threads used by the concurrent optimizer which can be switched on using the option **MIP Start Algorithm** .



**Note** 

*	The value of this option is limited by the number of available processors.




**Learn more about** 

*	:ref:`option-ODHCPLEX-auxiliary_root_threads` 
*	:ref:`option-ODHCPLEX-mip_start_algorithm` 
*	:ref:`option-ODHCPLEX-parallel_mode` 



