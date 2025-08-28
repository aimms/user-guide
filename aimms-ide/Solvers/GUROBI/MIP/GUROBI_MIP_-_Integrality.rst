.. _option-GUROBI-integrality:


Integrality
===========



:Type:	Floating point number	
:Range:	[1e-9,0.1]	
:Default:	1e-5	



This option specifies the integer feasibility tolerance (MIP only). An integrality restriction on a variable is considered satisfied when the difference between the variable's value and the nearest integer value is smaller than the value of this option.



If this option is set too small, Gurobi may falsely conclude that the problem is infeasible.



**Note** 

*	Another reason why Gurobi may falsely conclude that a problem is infeasible, is if the option **Feasibility**  is set too low.




**Learn more about** 

*	:ref:`option-GUROBI-feasibility`  
*	:ref:`option-GUROBI-integrality_focus`  



