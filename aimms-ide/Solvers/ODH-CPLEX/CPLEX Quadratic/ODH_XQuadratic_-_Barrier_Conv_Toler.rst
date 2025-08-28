.. _option-ODHCPLEX-barrier_convergence_tolerance_for_qcp:


Barrier Convergence Tolerance for QCP
=====================================



:Type:	Floating point number	
:Range:	[1e-12,inf)	
:Default:	1e-7	



This option determines the convergence tolerance for QCP (quadratically constrained problems). It sets the tolerance on complementarity for convergence. The barrier algorithm terminates with an optimal solution if the relative complementarity is smaller than this value.



Changing this tolerance to a smaller value may result in greater numerical precision of the solution, but also increases the chance of a convergence failure in the algorithm and consequently may result in no solution at all. Therefore, caution is advised in deviating from the default setting.



**Note** 

*	For LPs and QPs (that is, when all constraints are linear) see the option **Barrier Convergence Tolerance**.




**Learn more about** 

*	:ref:`option-ODHCPLEX-barrier_convergence_tolerance` 



