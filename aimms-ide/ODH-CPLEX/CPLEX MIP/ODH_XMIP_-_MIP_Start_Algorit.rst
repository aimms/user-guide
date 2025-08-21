.. _option-ODHCPLEX-mip_start_algorithm:


MIP Start Algorithm
===================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Automatic	



The value of this option determines which LP algorithm should be used to solve the initial relaxation of the MIP. Possible values are:



*	Automatic
*	Primal simplex
*	Dual simplex
*	Network simplex
*	Barrier
*	Sifting
*	Concurrent




Sifting solves a sequence of LP subproblems, where the results from one subproblem are used to select columns from the original model for inclusion in the next subproblem. This iterative sifting process eventually converges to an optimal solution for the original model. Sifting is especially applicable to models with many more columns than rows.





On a multiprocessor computer, the concurrent optimizer launches distinct LP optimizers on multiple threads to solve the initial relaxation of the MIP, terminating as soon as the first optimizer finishes. The amount of threads available to the concurrent optimizer is controlled by the option **Global Thread Limit** .





The concurrent optimizer requires more memory than any individual optimizer, and of course it adds system load by consuming more aggregate CPU time than the fastest individual optimizer would alone. However, the advantages offered in terms of robust solution of models, and assurance in most cases of the minimum solution time, will make it attractive in many situations.





**Note** 

*	The option **MIP Method**  determines which continuous optimizer will be used to solve the subproblems in a MIP, after the initial relaxation.




**Learn more about** 

*	:ref:`option-ODHCPLEX-global_thread_limit`  
*	:ref:`option-ODHCPLEX-mip_method` 
