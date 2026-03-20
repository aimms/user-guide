.. _option-CPOPT-relative_optimality_tolerance:


Relative Optimality Tolerance
=============================



:Type:	Floating point number	
:Range:	[0,1]	
:Default:	1e-4	



This option sets a relative tolerance on the objective value for optimization models. This means that when CP Optimizer reports an optimal solution found, then there is no solution which improves the objective by more than the absolute value of the objective times the value of this option. The default value of this option is 1e-4.



This option is used in conjunction with option **Optimality Tolerance**. The optimality of a solution is proven if either of the two options' criteria are fulfilled.



**Learn more about** 

*	:doc:`CPOPT_General_-_Optimality_tolerance` 
