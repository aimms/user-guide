

.. _option-IPOPT-ma27_real_workspace_memory:


MA27 real workspace memory
==========================



:Type:	Floating point number	
:Range:	[1,1e+019]	
:Default:	5	



This option determines the real workspace memory for MA27. The initial real workspace memory equals the memory required by the unfactored system multiplied by the value of this option. IPOPT will increase the workspace size by the value of the option **MA27 Increment Factor for Workspace Size**  if required.



**Note** 

*	This option is only used if the user has provided a DLL with HSL subroutines and if the option **Linear Solver Selection**  has been set to 'HSL routine MA27'. 




**Learn more about** 

*	:ref:`option-IPOPT-linear_solver_selection` 
*	:ref:`option-IPOPT-ma27_increment_factor_for_workspace_size` 
*	:ref:`option-IPOPT-ma27_integer_workspace_memory` 
