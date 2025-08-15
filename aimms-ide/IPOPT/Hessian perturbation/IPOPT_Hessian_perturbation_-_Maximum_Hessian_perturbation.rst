

.. _IPOPT_Hessian_perturbation_-_Maximum_Hessian_perturbation:


Maximum Hessian perturbation
============================



**Type**:	Floating point number	

**Range**:	[0,1e+019]	

**Default**:	1e+019	



This option determines the maximum value of regularization parameter for handling negative curvature. In order to guarantee that the search directions are indeed proper descent directions, IPOPT requires that the inertia of the (augmented) linear system for the step computation has the correct number of negative and positive eigenvalues. The idea is that this guides the algorithm away from maximizers and makes IPOPT more likely converge to first order optimal points that are minimizers. If the inertia is not correct, a multiple of the identity matrix is added to the Hessian of the Lagrangian in the augmented system. This parameter gives the maximum value of the regularization parameter. If a regularization of that size is not enough, the algorithm skips this iteration and goes to the restoration phase.

