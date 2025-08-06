.. _ODH-CPLEX_-_Parallel_Execution:


Parallel Execution
==================

**Description** 

ODH-CPLEX can use multiple simultaneous threads. ODH-CPLEX must use separate threads for the main CPLEX solve and for the ODH engine. Thus the processing capability of multi-core hardware can be exploited effectively.



Whilst there are good defaults for allocating available threads, it may be worthwhile to give some attention to the allocation of threads between the main CPLEX solver and the ODH engine for ODH-CPLEX.



If the option **Thread Limit**  is set then its value sets the number of threads that are allocated in total, otherwise the total number of threads allocated for ODH-CPLEX is set to the number of physical processors available on the computer. If the option **Thread Limit**  is set to a number greater than the number of available processors, multiple threads will have to share the same processor, which may severely degrade performance.



In general, the more threads allocated to the main CPLEX solver, the faster it will run, and similarly, the more allocated to the ODH engine, the faster it will run. The best balance depends on the model being solved and whether it is intended to run to optimality or to an optimality gap of (say) 5% or 10%. If the **Global Thread Limit**  is at its default value (of 0), ODH-CPLEX defaults to allocating a quarter of the threads to the ODH engine and the remainder to the main CPLEX solve. Otherwise it allocates **Global Thread Limit**  threads to the main CPLEX solver and the remainder to the ODH engine.



Within the ODH engine, the principal heuristic algorithm can run in parallel on multiple threads. Each algorithmic thread uses CPLEX to solve sub-models and each such instance of CPLEX can itself run on multiple threads. So some attention needs to be given to the allocation of threads between them. If SUB_CPX_THREADS is not set, the CPLEX solver will use one thread for each available logical processor to solve the sub-models. This means that only one thread will be available for the solution improvement heuristic. If the option SUB_CPX_THREADS is set, then by default the heuristic engine sets its number of algorithmic threads to



	number_of_available_processors / SUB_CPX_THREADS



where number_of_available_processors is: the number of logical processors if the **Search Mode**  equals 'Feasible solution'; and this number less those allocated to the main CPLEX solver if the **Search Mode**  equals 'Optimal solution'.



SUB_CPX_THREADS is a CPLEX option that only applies to CPLEX when it solves a sub-model. Is can only be set using a :ref:`ODH-CPLEX_-_Parameter_File` .



Many Intel and compatible processors support hyperthreading (where this is enabled on the computer and operating system) and if so there will be two logical processors for every physical core. Using them can severely degrade performance, so if they are enabled it is often a good idea to set **Thread Limit**  to the number of physical processors. Note that on machines with a large number of processors (cores), the principal bottleneck for large scale optimization is usually memory access. In practice it is often better to use only about half of the available cores on (say) a 24 core Intel Xeon system. This is model dependent and some experimentation is worthwhile.



Although the operating system’s scheduler usually allocates threads to logical processors so that they run on separate physical cores where possible, it will have more threads to manage than those of the heuristic or CPLEX and so will change this allocation as the heuristic and CPLEX run so as to balance its workload effectively. There is a performance penalty to doing this from the perspective of the heuristic run time. For the ODHeuristics stand-alone, used if the **Search Mode**  equals 'Feasible solution', this can be avoided by locking the heuristic threads to specific processors by setting the heuristic option **Processor Lock**  to 1. It is not supported if the **Search Mode**  equals 'Optimal solution' Under Windows, beware that the threads need to be locked at an above normal priority so this may have a negative impact on other programs concurrently running on the machine.



**Learn more about** 

*	:ref:`ODH-CPLEX_XPar_-_GlobalThreadLimit` 
*	:ref:`ODH-CPLEX_-_Parameter_File` 
*	:ref:`ODH-CPLEX_Parallel_-_Processor_Lock` 
*	:ref:`ODH-CPLEX_General_-_Search_Mode` 
*	:ref:`ODH-CPLEX_Parallel_-_Thread_Limit` 
