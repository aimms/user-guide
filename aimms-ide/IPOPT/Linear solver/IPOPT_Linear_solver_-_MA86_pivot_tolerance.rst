

.. _option-IPOPT-ma86_pivot_tolerance:


MA86 pivot tolerance
====================



:Type:	Floating point number	
:Range:	[0,0.5]	
:Default:	1e-008	



This option specifies the pivot tolerance for the linear solver MA86. A smaller number pivots for sparsity, a larger number pivots for stability.



**Note** 

*	This option is only used if the user has provided a DLL with HSL subroutines and if the option **Linear Solver Selection**  has been set to 'HSL_MA86'. 




**Learn more about** 

*	:ref:`option-IPOPT-linear_solver_selection` 
*	:ref:`option-IPOPT-ma86_maximum_pivot_tolerance` 
