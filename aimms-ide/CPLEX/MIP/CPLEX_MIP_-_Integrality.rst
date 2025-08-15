.. _CPLEX_MIP_-_Integrality:


Integrality
===========



:Type:	Floating point number	
:Range:	[0.0,0.5]	
:Default:	1e-5	



The setting of this option specifies the amount by which an integer variable can be different than an integer and still be considered feasible. If this option is set too small, CPLEX may falsely conclude that the problem is infeasible.



**Note** 

*	Another reason why CPLEX may falsely conclude that a problem is infeasible, is if the option **Feasibility**  is set too low.
*	CPLEX does not automatically reset the value of the option **Feasibility**  to be less than or equal to the value of this option.




**Learn more about** 

*	:ref:`CPLEX_Simplex_-_Feasibility`  



