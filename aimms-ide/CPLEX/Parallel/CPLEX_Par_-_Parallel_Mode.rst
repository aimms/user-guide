.. _CPLEX_Par_-_Parallel_Mode:


Parallel Mode
=============



**Type** :	Selection	

**Range** :	The settings listed below	

**Default** :	Automatic	



This option determines the parallel optimization mode. Possible values are:



*	Opportunistic
*	Automatic
*	Deterministic




In this context, deterministic means that multiple runs with the same model at the same option settings on the same platform will reproduce the same solution path and results. In contrast, opportunistic implies that even slight differences in timing among threads or in the order in which tasks are executed in different threads may produce a different solution path and consequently different timings or different solution vectors during optimization executed in parallel threads. In multithreaded applications, the opportunistic setting entails less synchronization between threads and consequently may provide better performance. 





By default, CPLEX applies as much parallelism as possible while still achieving deterministic results. That is, when you run the same model twice on the same platform with the same option settings, you will see the same solution and optimization run. This condition is referred to as the deterministic mode.





**Deterministic and sequential optimization** 





More opportunities to exploit parallelism are available if you do not require determinism. In other words, CPLEX can find more opportunities for parallelism if you do not require an invariant, repeatable solution path and precisely the same solution vector. To use all available parallelism, you need to select the opportunistic parallel mode. In this mode, CPLEX will utilize all opportunities for parallelism in order to achieve best performance. However, in opportunistic mode, the actual optimization may differ from run to run, including the solution time itself and the path traveled in the search.





Parallel MIP optimization can be opportunistic or deterministic. Parallel barrier optimization is only deterministic. Consequently, when the parallel mode is set to opportunistic, barrier optimization is restricted to run only sequentially, not in parallel.





Concurrent optimization can be opportunistic or deterministic. In either mode, when six or more threads are available, concurrent optimization launches primal simplex, dual simplex, and barrier optimizers by default. If ten threads are available to CPLEX, concurrent optimization launches primal simplex, dual simplex, barrier, and sifting (if sifting is applicable to the current type of problem). The concurrent optimizer is described in the section :ref:`CPLEX_Parallel_Concurrent_Optimizer` .





**Callbacks and MIP optimization** 





If a branch, candidate, cut, heuristic or lazy constraint callback is used for solving a MIP then the order in which the callbacks are called cannot be guaranteed to remain deterministic, not even in deterministic mode. Thus, to make sure of deterministic runs when this **Parallel Mode**  option and the **Global Thread Limit**  option are at their default settings, CPLEX reverts to sequential solving of the MIP. That is, CPLEX will then use only one thread. If the option **Use Generic Callbacks**  is set to 'Yes' then CPLEX will use multiple threads in this situation but also in that case the behavior is not deterministic, even in deterministic mode (with the only exception of having only a heuristic callback installed).





**Determinism versus opportunism** 





Cases where you might wish to turn off deterministic search include situations where you want to take advantage of possibly faster performance of opportunistic parallel MIP optimization in multiple threads after you have confirmed that deterministic parallel MIP optimization produced the results you expected.





**Note** 

*	If the **Global Thread Limit**  is set to a value greater than 1, and a branch, candidate, cut, heuristic or lazy constraint callback is installed, then the behavior will be opportunistic even if the deterministic mode is used. (If only a heuristic callback is installed and the option **Use Generic Callbacks**  is set to 'Yes' then the behavior will be deterministic.)
*	If the deterministic mode is used then AIMMS might become less responsive and the Progress Window might be updated less frequently.




**Learn more about** 

*	:ref:`CPLEX_Threads_search_strat_and_callb` 
*	:ref:`CPLEX_Par_-_GlobalThreadLimit` 
*	:ref:`CPLEX_Parallel_Concurrent_Optimizer` 
*	:ref:`CPLEX_MIP_-_Use_Generic_Callbacks` 



