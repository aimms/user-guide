.. _CONOPT_Stop_Criteria_-_Slow_Progress_Tol:

Slow Progress Tolerance
=======================



**Type**:	Floating point number	

**Range**:	[3e-13,1e-5]

**Default**:	3e-12	



This option determines the slow progress tolerance. The change in the objective value in a well-behaved iteration is considered small if it is less than the value of this option* max(1,|fobj|), where fobj is the value of the current objective function. The value is used in tests for "Slow Progress"; see the option **Limit for Slow Progress** .



**Learn more about** 

*	:ref:`CONOPT_Stop_Criteria_-_Limit_Slow_Progress`  






