.. _CONOPT_Stop_Criteria_-_Optimality_Tol_Infeasible:

Optimality Tolerance Infeasible
===============================



:Type:	Floating point number	
:Range:	[3e-13,1]
:Default:	1e-7



This option specifies the optimality tolerance for the reduced gradient when the solution is infeasible. The reduced gradient is considered zero and the solution infeasible if the largest superbasic component if the reduced gradient is less than the value of this option.



