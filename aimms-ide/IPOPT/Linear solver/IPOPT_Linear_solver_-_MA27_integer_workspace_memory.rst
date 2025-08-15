

.. _IPOPT_Linear_solver_-_MA27_integer_workspace_memory:


MA27 integer workspace memory
=============================



:Type:	Floating point number	
:Range:	[1,1e+019]	
:Default:	5	



This option determines the integer workspace memory for MA27. The initial integer workspace memory equals the memory required by the unfactored system multiplied by the value of this option. IPOPT will increase the workspace size by the value of the option **MA27 Increment Factor for Workspace Size**  if required.



**Note** 

*	This option is only used if the user has provided a DLL with HSL subroutines and if the option **Linear Solver Selection**  has been set to 'HSL routine MA27'. 




**Learn more about** 

*	:ref:`IPOPT_Linear_solver_-_Linear_solver_selection` 
*	:ref:`IPOPT_Linear_solver_-_MA27_increment_factor_for_workspace_size` 
*	:ref:`IPOPT_Linear_solver_-_MA27_real_workspace_memory` 
