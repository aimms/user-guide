

.. _option-IPOPT-mumps_maximum_pivot_tolerance:


MUMPS maximum pivot tolerance
=============================



:Type:	Floating point number	
:Range:	[0,1]	
:Default:	0.1	



This option specifies the maximum pivot tolerance for the linear solver MUMPS. IPOPT may increase the pivot tolerance as high as the value of this option to get a more accurate solution to the linear system.



**Note** 

*	This option is only used if the option **Linear Solver Selection**  has been set to 'MUMPS solver'. 




**Learn more about** 

*	:ref:`option-IPOPT-linear_solver_selection` 
*	:ref:`option-IPOPT-mumps_pivot_tolerance` 
