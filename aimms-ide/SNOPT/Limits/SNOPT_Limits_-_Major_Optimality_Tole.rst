.. _SNOPT_Limits_-_Major_Optimality_Tole:


Major Optimality Tolerance
==========================



**Type**:	Floating point number	

**Range**:	[0,1000]	

**Default**:	1e-6	



This option specifies the final accuracy of the dual variables. On successful termination, SNOPT will have computed a solution (x,s,p) such that maximum complementarity gap for each variable, divided by the norm of the dual variables p, is smaller than or equal to the value of this option. The complementarity gaps are computed from the final QP solution using the reduced gradients.



**Learn more about** 

*	:ref:`SNOPT_Limits_-_Optimality_Tolerance`  



