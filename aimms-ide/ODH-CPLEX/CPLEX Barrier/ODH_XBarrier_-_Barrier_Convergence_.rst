.. _ODH-CPLEX_XBarrier_-_Barrier_Convergence_:


Barrier Convergence Tolerance
=============================



:Type:	Floating point number	
:Range:	[1e-12,inf)	
:Default:	1e-8	



This option can be used to set the tolerance on complementarity for convergence. The barrier algorithm will terminate with an optimal solution if the relative complementarity is smaller than this value.



Changing this tolerance to a smaller value may result in greater numerical precision of the solution, but also increases the chance of a convergence failure in the algorithm and consequently may result in no solution at all. Therefore, caution is advised in deviating from the default setting.



**Note** 

*	For problems with quadratic constraints (QCP) see the option **Barrier Convergence Tolerance for QCP** .




**Learn more about** 

*	:ref:`ODH-CPLEX_XQuadratic_-_Barrier_Conv_Toler` 



