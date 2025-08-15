.. _MINOS_-_Maximum_Number_of_Min:


Maximum Number of Minor Iterations
==================================



**Type**:	Integer	

**Range**:	{1..10000000}	

**Default**:	40	



This is the maximum number of minor iterations allowed between successive linearizations of the nonlinear constraints. A moderate value (e.g., 10 ≤ k ≤ 50) prevents excessive effort being expended on early major iterations, but allows later subproblems to be solved to completion.



In general it is unsafe to specify a value as small as k = 1 or 2. (Even when an optimal solution has been reached, a few minor iterations may be needed for the corresponding subproblem to be recognized as optimal.)



Note that the global solvers option **Iteration Limit**  defines (in case of MINOS) an independent limit on the number of major iterations. (A major iteration consists of a linearization of the nonlinear constraints.)



**Learn more about** 

*	:ref:`Options_Stop_Criteria_-_Iteration_Limi`  
*	:ref:`MINOS_Limits_-_Maximum_Number_of_Tot`  



