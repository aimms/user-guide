

.. _PenaltyParameter:
.. _MINOS_PenaltyParameter:


Penalty Parameter
=================



**Type** :	Floating point number	

**Range** :	[0,1e20]	

**Default** :	2000	



This option specifies the initial value of the penalty parameter r in the modified augmented Lagrangian. The penalty parameter r will be set equal to the value of this option devided by the number of nonlinear constraints.



For early runs on a problem with unknown characteristics, something like the default value should be specified. If the problem is known to be highly nonlinear, specify a larger value, such as 10 times the default. In general, a positive value of r may be necessary to ensure convergence, even for convex programs.



On the other hand, if r is too large, the rate of convergence may be unnecessarily slow. If the functions are not highly nonlinear or a good starting point is known, it will often be safe to set the value of this option equal to 0.0.



If several related problems are to be solved, the following strategy for setting the penalty parameter may be useful:

1.	Initially, use a moderate value for r (such as the default) and a reasonably low value for **Maximum Number of Total Iterations**  and/or **Iterations Limit** .

2.	If successive major iterations appear to be terminating with radically different solutions, the penalty parameter should be increased. (See also the **Damping Parameter** .)

3.	If there appears to be little progress between major iterations, the penalty parameter could be reduced.



**Learn more about** 

*	:ref:`MINOS_DampingParameter`  
*	:ref:`MINOS_Limits_-_Maximum_Number_of_Tot`  
*	:ref:`MINOS_RadiusofConvergence`  
