.. _KNITRO_Advanced_-_SolutionProgressTol:


Solution Progress Tolerance
===========================



**Type**:	Floating point number	

**Range**:	[0,1]	

**Default**:	1e-12	



The optimization will terminate when the relative change in the solution estimate is less than the value of this option for n consecutive iterations, where n is the value of the option **Solution Progress Iterations** . When using an interior-point algorithm and the barrier parameter is still large, Knitro will first try decreasing the barrier parameter before terminating.



**Learn more about** 

*	:ref:`KNITRO_Advanced_-_Solution_Progress_Iterations` 



