

.. _IPOPT_Linear_solver_-_MA97_pivot_tolerance:


MA97 pivot tolerance
====================



:Type:	Floating point number	
:Range:	[0,0.5]	
:Default:	1e-008	



This option specifies the pivot tolerance for the linear solver MA97. A smaller number pivots for sparsity, a larger number pivots for stability.



**Note** 

*	This option is only used if the user has provided a DLL with HSL subroutines and if the option **Linear Solver Selection**  has been set to 'HSL_MA97'. 




**Learn more about** 

*	:ref:`IPOPT_Linear_solver_-_Linear_solver_selection` 
*	:ref:`IPOPT_Linear_solver_-_MA97_maximum_pivot_tolerance` 
