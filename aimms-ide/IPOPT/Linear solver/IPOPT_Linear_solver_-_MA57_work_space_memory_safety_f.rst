

.. _IPOPT_Linear_solver_-_MA57_work_space_memory_safety_f:


MA57 work space memory safety factor
====================================



**Type**:	Floating point number	

**Range**:	[1,1e+019]	

**Default**:	3	



This option determines the safety factor for work space memory allocation for the linear solver MA57. If 1 is chosen, the suggested amount of work space is used. However, choosing a larger number might avoid reallocation if the suggest values do not suffice. 



**Note** 

*	This option is only used if the user has provided a DLL with HSL subroutines and if the option **Linear Solver Selection**  has been set to 'HSL routine MA57'. 




**Learn more about** 

*	:ref:`IPOPT_Linear_solver_-_Linear_solver_selection` 
