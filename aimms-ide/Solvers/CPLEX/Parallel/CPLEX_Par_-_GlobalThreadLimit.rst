.. _option-CPLEX-global_thread_limit:


Global Thread Limit
===================



:Type:	Integer	
:Range:	{0 .. 2100000000}	
:Default:	0	



This option sets the maximal number of parallel threads that will be invoked by any CPLEX parallel optimizer. This
option interacts with the Parallel Mode option. CPLEX can use parallel threads for solving MIP models and, if the
barrier algorithm is used, for solving LP, QP and QCP models.


For a single thread, the parallel algorithms behave deterministically, regardless of thread option settings; that is,
the algorithm proceeds sequentially in a single thread.


In this context, sequential means that the algorithm proceeds step by step, consecutively, in a predictable and
repeatable order within a single thread. *Deterministic* means that repeated solving of the same model with the same
option settings on the same computing platform will follow exactly the same solution path, yielding the same level
of performance and the same values in the solution. Sequential execution is deterministic. In multithreaded computing,
a deterministic setting requires synchronization between threads. *Opportunistic* entails less synchronization between
threads and thus may offer better performance at the sacrifice of repeatable, invariant solution paths and values in
repeated runs on multiple threads or multiple processors.


When this option is at its default setting 0, and your application includes no callbacks or only informational callbacks,
CPLEX can use all available threads; that is, at most 32 threads or the number of cores of the machine, whichever is smaller.
If your machine offers more than 32 threads, you can take advantage of them by increasing the value of this option.


When this option is at its default setting 0, and your application includes a branch, candidate, cut, heuristic or lazy constraint
callback, then CPLEX uses one thread. In other words, the presence of a branch, candidate, cut, heuristic or lazy constraint
callback turns off parallel processing when the value of this option is at its default.


In order to use parallel optimization in conjunction with a branch, candidate, cut, heuristic or lazy constraint callbacks, you
need to set this option to a positive value. However, when you do so, you need to be aware of the fact that the callbacks may be
invoked concurrently, and that the algorithm might become opportunistic even if the option **Parallel Mode** is set to
'Deterministic'. This only holds if the option **Use Generic Callbacks** is set to 'No'.


This option also determines the amount of threads used by the concurrent optimizer which can be switched on using the option
**LP Method** or **MIP Start Algorithm**. The concurrent optimizer is described in the section :ref:`CPLEX_Parallel_Concurrent_Optimizer`.


**Note** 

*	The value of this option is limited by the number of available processors.


**Learn more about** 

*	:ref:`option-CPLEX-auxiliary_root_threads` 
*	:ref:`CPLEX_Threads_search_strat_and_callb` 
*	:ref:`option-CPLEX-lp_method` 
*	:ref:`option-CPLEX-mip_start_algorithm` 
*	:ref:`CPLEX_Parallel_Concurrent_Optimizer` 
*	:ref:`option-CPLEX-parallel_mode` 
*	:ref:`option-CPLEX-use_generic_callbacks` 

