.. _KNITRO_Term_-_AbsOptTol:


Absolute Optimality Tolerance
=============================



**Type**:	Floating point number	

**Range**:	[0,1e20]	

**Default**:	0.001	



This option specifies the final absolute stopping tolerance for the KKT (optimality) error. Smaller values for this option result in a higher degree of accuracy in the solution with respect to optimality.



The feasibility error is defined as the maximum violation among all constraints. It is 0 if there are no constraint violations.



**Learn more about** 

*	:ref:`KNITRO_Term_-_RelOptTol`  
