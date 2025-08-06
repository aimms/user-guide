.. _KNITRO_Term_-_RelOptTol:


Relative Optimality Tolerance
=============================



**Type** :	Floating point number	

**Range** :	[0,1]	

**Default** :	1e-6	



This option specifies the final absolute stopping tolerance for the KKT (optimality) error. Smaller values for this option result in a higher degree of accuracy in the solution with respect to optimality. The value 0.0 has a special meaning; for that setting Knitro does not use the relative optimality tolerance.



The feasibility error is defined as the maximum violation among all constraints. It is 0 if there are no constraint violations. As scaling factor for the relative stopping tolerance Knitro uses



	t2 = max( 1, ``||``  Ñ f(xk,yk) ``||`` ¥ )



if the problem is constrained, and



	t2 = max( 1, min( | f(xk,yk) | , ``||``  Ñ f(x0,y0) ``||`` ¥ ) )



if the problem is unconstrained. Here f represents the objective function.



**Learn more about** 

*	:ref:`KNITRO_Term_-_AbsOptTol`  
