

.. _CPX221_Parallel_Concurrent_Optimizer:
.. _CPLEX_Parallel_Concurrent_Optimizer:


Parallel Concurrent Optimizer
=============================

For solving an LP model or the initial relaxation of an MIP model CPLEX can use different algorithms as controlled by the options **LP Method**  and **MIP Start Algorithm**  respectively. One of these algorithms is the concurrent optimizer.



On a multiprocessor computer, the concurrent optimizer launches distinct LP optimizers on multiple threads to solve the initial relaxation of the MIP, terminating as soon as the first optimizer finishes. The first thread uses the dual simplex algorithm. If a second thread is available, the concurrent optimizer runs the barrier optimizer on it.



In the presence of more than three threads (for example, on hardware with four or more processors), the behavior of the concurrent optimizer depends on whether the **Parallel Mode**  is opportunistic or deterministic. If the parallel mode is opportunistic and a third processor is available, the concurrent optimizer runs all three optimizers simultaneously: dual simplex, primal simplex, and barrier. All further available threads are devoted to making the barrier optimization parallel. In contrast, if the parallel mode is deterministic (the default mode) and 2 to 5 threads are available, then the concurrent optimizer runs the dual simplex and barrier optimizers simultaneously, and if at least 6 threads are available then the concurrent optimizer runs the dual simplex, primal simplex and barrier optimizers simultaneously; all additional threads are applied to making the barrier optimizer parallel.



If you invoke concurrent optimization on an LP model, the concurrent optimizer checks the ratio between variables and constraints in the model. If the concurrent optimizer finds a large ratio, and if 10 or more threads are available to CPLEX, then the concurrent optimizer also invokes sifting on the LP model.



The amount of threads available to the concurrent optimizer is controlled by the option **Global Thread Limit** .



**Finishing first: basis solution in concurrent optimization** 

Barrier optimization is not considered complete until the crossover step has been performed and simplex re-optimization has converged; in other words, regardless of which optimizer turns out to be the fastest, the concurrent optimizer always returns a basis solution at optimality.



**Performance trade-offs in concurrent optimization** 

The concurrent optimizer requires more memory than any individual optimizer, and of course it adds system load by consuming more aggregate CPU time than the fastest individual optimizer would alone. However, the advantages offered in terms of robust solution of models, and assurance in most cases of the minimum solution time, will make it attractive in many situations.



**Interpreting the log in concurrent optimization** 

When you invoke concurrent optimization in your application, you may observe a point in the CPLEX log file when CPLEX reports a solution of the model by an optimizer, but no other report of activity appears in the log for a considerable time afterward. During this apparently inactive period, concurrent optimization deterministically manages potential race conditions among competing optimizers. Among other decisions during this period, the concurrent optimizer decides deterministically from which of those competing optimizers to accept the final solution.



If this apparent wait during the race between concurrent optimizers poses a problem for your application, there are two alternative remedies available to you:




*   Use opportunistic mode, rather than the default deterministic mode. To do so, change the setting of the **Parallel Mode**  option.
*   Set the optimizer that consistently solves your model first as the starting algorithm in your application. To do so, set the option appropriate for your type of model: **LP Method**  or **MIP Start Algorithm** .



**Learn more about** 

*	:ref:`CPLEX_Par_-_GlobalThreadLimit` 
*	:ref:`CPLEX_General_-_LP_Method` 
*	:ref:`CPLEX_MIP_-_MIP_Start_Algorit` 
*	:ref:`CPLEX_Par_-_Parallel_Mode` 
