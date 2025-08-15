.. _SNOPT_Advanced_-_Elastic_Weight:


Elastic Weight
==============



:Type:	Floating point number	
:Range:	[0,1e10]	
:Default:	1e6	



If a QP is infeasible or unbounded (or if the dual variables for the nonlinear constraints become too large), SNOPT enters an "elastic" mode in which the nonlinear constraint violations are added to the objective function and penalized by using a constant. The QP created in this way is resolved by setting this constant equal to the elastic weight (i.e., the value of this option) multiplied by the norm of the objective gradient.



(The constant is increased later on by multiplying it by 10 every time the optimal solution of the "elastic problem" is not feasible for the original problem.)



