.. _option-GUROBI-method:


Method
======



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Automatic	



This option determines which algorithm should be used when solving continuous models or the root node of a MIP model. Possible values are:



    *	Automatic
    *	Primal simplex
    *	Dual simplex
    *	Barrier
    *	Opportunistic concurrent
    *	Deterministic concurrent




Setting 'Automatic' means that barrier is used for solving a QP model, and dual simplex otherwise. Only primal and dual simplex are available for solving the root of an MIQP model.





Concurrent optimization is a simple approach for exploiting multiple processors. It starts multiple, independent solves on a model, using different strategies for each. Optimization terminates when the first one completes. By pursuing multiple different strategies simultaneously, the concurrent optimizer can often obtain a solution faster than it would if it had to choose a single strategy.





The first concurrent thread is devoted to dual simplex, the second through fourth to a single parallel barrier solve, and the fifth to primal simplex. Additional threads are devoted to the one parallel barrier solve. Thus, for example, a concurrent LP solve using four threads would devote one thread to dual simplex and three to parallel barrier. The number of threads used by the concurrent optimizer is limited by the option **Thread Limit** .





Setting 'Deterministic concurrent' gives the exact same result each time, while setting 'Opportunistic concurrent' is often faster but can produce different optimal solutions when run multiple times.





**Note** 

*	The option **MIP Node Method**  determines which algorithm should be used when solving node relaxations within the MIP solver.
*	This option also determines the method used for solving the LP model (if any) during the postsolve.
*	The option **Sensitivity Method**  determines which method is used by Gurobi for solving LP problems while calculating sensitivity ranges.
*	The option **Concurrent Method**  controls the methods used by the concurrent solver when solving an LP.




**Learn more about** 

*	:ref:`option-GUROBI-concurrent_method` 
*	:ref:`option-GUROBI-mip_node_method` 
*	:ref:`option-AIMMS-postsolve` 
*	:ref:`option-GUROBI-sensitivity_method` 
*	:ref:`option-GUROBI-thread_limit` 



