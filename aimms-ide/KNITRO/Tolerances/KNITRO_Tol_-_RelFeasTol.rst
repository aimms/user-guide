.. _KNITRO_Tol_-_RelFeasTol:


Relative Feasibility Tolerance
==============================



**Type**:	Floating point number	

**Range**:	[0,1]	

**Default**:	1e-6	



This option specifies the final relative stopping tolerance for the feasibility error. Smaller values for this option result in a higher degree of accuracy in the solution with respect to feasibility. The value 0.0 has a special meaning; for that setting Knitro does not use the relative feasibility tolerance.



The feasibility error is defined as the maximum violation among all constraints. It is 0 if there are no constraint violations. As scaling factor for the relative stopping tolerance Knitro uses



	t1 = max( 1, gj(x0,y0) - Uj, Lj - gj(x0,y0) ),



where (x0,y0) represents the initial point, g the constraint functions, and L and U the lower and upper bounds on g. I.e., the maximum violation among all constraints in the initial point (with a minimum of 1).



**Learn more about** 

*	:ref:`KNITRO_Tol_-_AbsFeasTol`  
