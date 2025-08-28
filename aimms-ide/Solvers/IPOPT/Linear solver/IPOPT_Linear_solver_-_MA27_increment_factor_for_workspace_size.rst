

.. _option-IPOPT-ma27_increment_factor_for_workspace_size:

MA27 increment factor for workspace size
========================================



:Type:	Floating point number	
:Range:	[1,1e+019]	
:Default:	10	



This option determines the increment factor for the workspace size for MA27. If the integer or real workspace is not large enough, IPOPT will increase its size by this factor.



**Note** 

*	This option is only used if the user has provided a DLL with HSL subroutines and if the option **Linear Solver Selection**  has been set to 'HSL routine MA27'. 




**Learn more about** 

*	:ref:`option-IPOPT-linear_solver_selection` 
*	:ref:`option-IPOPT-ma27_integer_workspace_memory` 
