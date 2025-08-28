.. _option-GUROBI-maximal_variable_bound:


Maximal Variable Bound
======================



:Type:	Floating point number	
:Range:	[0.0,1e100]	
:Default:	1e100	



This option only applies to NLP and MINLP models.



If a variable has no upper bound then the upper bound passed to Gurobi will be equal to the value of this option. If a variable has no lower bound then the lower bound passed to Gurobi will be equal to the value of this option multiplied by -1.



For example, if you have a variable x1 with range [0,999999] and a variable x2 with range [0,inf) then this will be passed to Gurobi as variables x1 with range [0,999999] and x2 with range [0,1000] if the value of this option is set to 1000.



If the value of this option is set to 1e100 (or higher) then each infinite variable bound in AIMMS will be treated as an infinite variable bound by Gurobi. This is the default setting.



**Note** 

*	Gurobi requires that all nonlinear variables and expressions in the mathematical program are bounded from below and above. It is important that the user provides finite lower and upper bounds on the variables. If not, global optimality of the solution provided is sometimes not guaranteed.
*	Gurobi might return 'infeasible' if the value of this option is set too low.



