.. _CPOPT_General_-_Optimality_tolerance:


Optimality tolerance
====================



:Type:	Floating point number	
:Range:	[0,inf)	
:Default:	0



This option sets an absolute tolerance on the objective value for optimization models. This means that when CP Optimizer reports an optimal solution found, then there is no solution which improves the objective by more than the value of this option. The default value of this option is 0.



This option is used in conjunction with option **Relative Optimality Tolerance** . The optimality of a solution is proven if either of the two options' criteria is fulfilled.



**Learn more about** 

*	:ref:`CPOPT_General_-_Relative_optimality_tolerance` 
