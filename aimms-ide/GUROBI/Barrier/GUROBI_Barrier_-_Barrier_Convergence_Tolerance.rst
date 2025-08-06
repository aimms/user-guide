.. _GUROBI_Barrier_-_Barrier_Convergence_Tolerance:


Barrier Convergence Tolerance
=============================



**Type** :	Floating point number	

**Range** :	[0,1]	

**Default** :	1e-8	



This option controls barrier termination. The barrier solver terminates when the relative difference between the primal and dual objective values is less than the specified tolerance.



Tightening this tolerance often produces a more accurate solution, which can sometimes reduce the time spent in crossover. Loosening it causes the barrier algorithm to terminate with a less accurate solution, which can be useful when barrier is making very slow progress in later iterations.



**Learn more about** 

*	:ref:`GUROBI_Barrier_-_Barrier_QCP_Convergence_Tol` 
