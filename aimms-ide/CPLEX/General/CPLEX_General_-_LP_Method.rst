.. _option-CPLEX-lp_method:


LP Method
=========



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Dual simplex	



For solving an LP, three methods can be applied: simplex, network in combination with simplex, and barrier. This option can be used to select combinations of solution methods. Possible values are:



*	Primal simplex
*	Dual simplex
*	Network + Primal (network followed by primal simplex)
*	Network + Dual (network followed by dual simplex)
*	Barrier
*	Sifting
*	Concurrent




Sifting solves a sequence of LP subproblems, where the results from one subproblem are used to select columns from the original model for inclusion in the next subproblem. This iterative sifting process eventually converges to an optimal solution for the original model. Sifting is especially applicable to models with many more columns than rows.





On a multiprocessor computer, the concurrent optimizer launches distinct LP optimizers on multiple threads, terminating as soon as the first optimizer finishes. The concurrent optimizer is described in the section :ref:`CPLEX_Parallel_Concurrent_Optimizer`. The amount of threads available to the concurrent optimizer is controlled by the option **Global Thread Limit** .





The concurrent optimizer requires more memory than any individual optimizer, and of course it adds system load by consuming more aggregate CPU time than the fastest individual optimizer would alone. However, the advantages offered in terms of robust solution of models, and assurance in most cases of the minimum solution time, will make it attractive in many situations.





**Note** 

*	If the setting 'Barrier' is chosen and the option **Solution Type**  is set to 'Nonbasic' then CPLEX will not provide a basic solution. Also, sensitivity information for objective coefficient ranges for variables and right-hand-side ranges for constraints will not be provided, and the sensitivity information for value ranges for variables and shadow price ranges for constraints will be meaningless.
*	The barrier algorithm can use parallel processes (threads) as controlled by the option **Global Thread Limit** .
*	This option also determines the LP method used for solving the LP model (if any) during the postsolve.
*	This option also determines the method used for solving a RMIP model.
*	The option **Sensitivity Method**  determines which method is used by CPLEX for solving LP problems while calculating sensitivity ranges.




**Learn more about** 

*	:ref:`option-CPLEX-global_thread_limit`  
*	:ref:`CPLEX_Parallel_Concurrent_Optimizer` 
*	:ref:`Options_Postsolve_-_Postsolve` 
*	:ref:`option-CPLEX-sensitivity_method` 
*	:ref:`option-CPLEX-solution_type` 



