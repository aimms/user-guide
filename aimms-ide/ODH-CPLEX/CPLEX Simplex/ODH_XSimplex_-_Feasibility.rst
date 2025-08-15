.. _ODH-CPLEX_XSimplex_-_Feasibility:


Feasibility
===========



**Type**:	Floating point number	

**Range**:	[1e-9,1e-4]	

**Default**:	1e-6	



The feasibility tolerance specifies the degree to which a problem's basic variables may violate their bounds. This tolerance influences the selection of an optimal basis and can be reset to a lower value when a problem is having difficulty maintaining feasibility during optimization. You may also wish to lower this tolerance after finding an optimal solution if there is any doubt that the solution is truly optimal. If the feasibility tolerance is set too low, CPLEX may falsely conclude that a problem is infeasible.



This option also controls indirectly the maximum constraint violation as it controls the bound violations on slack (or structural) variables.



**Note** 

*	With a MIP problem, CPLEX can also falsely conclude that a problem is infeasible if the option **Integrality**  is set too low.
*	With a MIP problem, CPLEX no longer automatically resets the value of this option to be less than or equal to the value of the option **Integrality** .




**Learn more about** 

*	:ref:`ODH-CPLEX_XMIP_-_Integrality`  



