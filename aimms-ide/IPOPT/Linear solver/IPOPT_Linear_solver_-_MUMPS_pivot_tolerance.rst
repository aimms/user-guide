

.. _IPOPT_Linear_solver_-_MUMPS_pivot_tolerance:


MUMPS pivot tolerance
=====================



:Type:	Floating point number	
:Range:	[0,1]	
:Default:	1e-6	



This option specifies the pivot tolerance for the linear solver MUMPS. A smaller number pivots for sparsity, a larger number pivots for stability.



**Note** 

*	This option is only used if the option **Linear Solver Selection**  has been set to 'MUMPS solver'. 




**Learn more about** 

*	:ref:`IPOPT_Linear_solver_-_Linear_solver_selection` 
*	:ref:`IPOPT_Linear_solver_-_MUMPS_maximum_pivot_tolerance` 
