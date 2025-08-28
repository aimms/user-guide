.. _CPLEX_Threads_search_strat_and_callb:


Callback Procedures
===================

Callback procedures (callbacks for short) allow you to monitor closely and to guide the behavior of the CPLEX optimizers. In particular, callbacks allow user code to be executed regularly during an optimization run.



AIMMS supports the following callback procedures: branch, candidate, cut, heuristic, incumbent, iterations, lazy constraints, status change and time. CPLEX offers two implementations of these callbacks, namely using generic callbacks or using legacy callbacks. So, for the incumbent callback there exists a generic implementation and a legacy implementation, and this holds for all other AIMMS callback procedures as well. The option **Use Generic Callbacks** controls which implementation is used by CPLEX.



For generic callback procedures there are no special cases, that is, they can be used in combination with dynamic search and, by default, CPLEX will use as many threads as possible. For legacy callback procedures this is different. The type of callback procedure installed (if any) influences the behavior of CPLEX. The behavior is also influenced by the options **MIP Search Strategy**  and **Global Thread Limit**. This section attempts to clarify the interaction between these options and callback procedures.



The remainder of this section describes the callback procedures using the legacy callback implementation, which is used if the option **Use Generic Callbacks**  is set to 'No' (the default).



We first distinguish informational callbacks from control callbacks. The callbacks for incumbent, iterations, status change and time are informational callbacks. These callbacks are used to retrieve certain information from CPLEX. The callbacks for branch, candidate, cut, heuristic and lazy constraints are control callbacks. Control callbacks allow you to control the branch & cut search during the optimization of MIP problems. Because control callbacks intervene in the search, control callbacks will be ignored if dynamic search is used.



Interaction of callbacks with search strategy




.. list-table::

   * - **Automatic** 
     - Dynamic search
     - Dynamic search
     - Branch-and-cut
   * - **Branch-and-cut** 
     - Branch-and-cut
     - Branch-and-cut
     - Branch-and-cut
   * - **Dynamic search** 
     - Dynamic search
     - Dynamic search
     - Dynamic search, control callbacks ignored




The table above shows that if the option **MIP Search Strategy**  is set to 'Automatic' (the default) then CPLEX will use dynamic search unless a control callback procedure has been installed in which case CPLEX will use branch-and-cut.



If the option **Global Thread Limit**  is set to a value N strictly greater than 0 then CPLEX will use N threads. The amount of threads that is used by CPLEX if the option **Global Thread Limit**  is set to 0 (the default) depends on the **MIP Search Strategy**  and the callback procedures that have been installed. The table below shows the amount of threads CPLEX will use for different combinations of callback types and search strategies, if the option **Global Thread Limit**  is set to 0. In this table, P denotes the number of available processors.



Number of threads used by default for combinations of callbacks and search strategy




.. list-table::

   * - **Automatic** 
     - min( P, 32 )
     - min( P, 32 )
     - 1
   * - **Dynamic search** 
     - min( P, 32 )
     - min( P, 32 )
     - 1
   * - **Branch-and-cut** 
     - 1
     - 1
     - 1




At the default setting of 0 for **Global Thread Limit**, the amount of threads that CPLEX will use is equal to the number of available processors, with a maximum of 32. However, if control callbacks are installed then by default CPLEX will only use 1 thread unless the **Global Thread Limit**  is set to a value strictly larger than 1. CPLEX does this to ensure deterministic behavior. If the **Global Thread Limit**  is set to 2 or more, and control callbacks have been installed, then CPLEX becomes non-deterministic (see the option **Parallel Mode** ).



The table also shows that if branch-and-cut is selected as the search strategy then CPLEX will use 1 thread only at the default setting of 0 for **Global Thread Limit**. If you want to use multiple threads for branch-and-cut then you have to set **Global Thread Limit**  to a value strictly larger than 1.



**Note** 

*	The control callbacks (i.e., the branch, candidate, cut, heuristic and lazy constraints callbacks) are not supported for multi-objective optimization.




**Learn more about** 

*	:ref:`option-CPLEX-global_thread_limit` 
*	:ref:`option-CPLEX-mip_search_strategy` 
*	:ref:`option-CPLEX-parallel_mode` 
*	:ref:`option-CPLEX-use_generic_callbacks` 
