.. _CONOPT_Advanced_-_Method_Reduced_Hessian:


Method for Reduced Hessian
==========================



**Type** :	Selection	

**Range** :	The settings listed below	

**Default** :	Geometric mean	



This option specifies the method for initializing the diagonal of the approximate reduced Hessian. Possible values are:



*	Geometric mean
*	Smallest




Each time a nonbasic variable is made superbasic a new row and column is added to the approximate reduced Hessian. The off-diagonal elements are set to zero and the diagonal to a value controlled by this option:





If the value equals 'Geometric mean': The new diagonal element is set to the geometric mean of the existing diagonal elements. This gives the new diagonal element an intermediate value and new superbasic variables are therefore not given any special treatment. The initial steps should be of good size, but build-up of second order information in the new sub-space may be slower. The larger diagonal element may also in bad cases cause premature convergence.





If the value equals 'Smallest': The new diagonal element is set to the minimum of the existing diagonal elements. This makes the new diagonal element small and the importance of the new superbasic variable will therefore be high. The initial steps can be rather small, but better second order information in the new sub-space should be build up faster.




