.. _COPT_General_-_Feasibility_tolerance:


Feasibility Tolerance
=====================



**Type** :	Floating point number	

**Range** :	[1e-9,1e-4]	

**Default** :	1e-6	



The (primal) feasibility tolerance specifies the degree to which a problem's basic variables may violate their bounds. This tolerance influences the selection of an optimal basis and can be reset to a lower value when a problem is having difficulty maintaining feasibility during optimization. You may also wish to lower this tolerance after finding an optimal solution if there is any doubt that the solution is truly optimal. If the feasibility tolerance is set too low, COPT may falsely conclude that a problem is infeasible.



