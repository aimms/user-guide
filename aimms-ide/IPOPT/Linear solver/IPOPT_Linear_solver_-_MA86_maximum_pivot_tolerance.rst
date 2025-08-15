

.. _IPOPT_Linear_solver_-_MA86_maximum_pivot_tolerance:


MA86 maximum pivot tolerance
============================



**Type**:	Floating point number	

**Range**:	[0,0.5]	

**Default**:	0.0001	



This option specifies the maximum pivot tolerance for the linear solver MA86. IPOPT may increase the pivot tolerance as high as the value of this option to get a more accurate solution to the linear system.



**Note** 

*	This option is only used if the user has provided a DLL with HSL subroutines and if the option **Linear Solver Selection**  has been set to 'HSL_MA86'. 




**Learn more about** 

*	:ref:`IPOPT_Linear_solver_-_Linear_solver_selection` 
*	:ref:`IPOPT_Linear_solver_-_MA86_pivot_tolerance` 
