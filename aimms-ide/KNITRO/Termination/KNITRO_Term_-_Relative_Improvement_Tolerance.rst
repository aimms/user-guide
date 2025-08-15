.. _KNITRO_Term_-_Relative_Improvement_Tolerance:


Relative Improvement Tolerance
==============================



**Type**:	Floating point number	

**Range**:	[0,1e20]	

**Default**:	1e-15	



The optimization process will terminate if the relative change in the objective function is less than ftol for n consecutive iterations. Here ftol denotes the value of this option, while n denotes the setting of the option **Relative Improvement Iterations** .



**Learn more about** 

*	:ref:`KNITRO_Term_-_Relative_Improvement_Iterations`  
