

.. _IPOPT_Quasi-Newton_-_Method_for_Hessian_computation:


Method for Hessian computation
==============================



**Type** :	Selection	

**Range** :	The settings listed below	

**Default** :	Automatic	



This option determines which kind of information for the Hessian of the Lagrangian function is used by the algorithm. Possible values are:



*	Automatic
*	Exact
*	Quasi-Newton




Setting 'Automatic' means that exact derivatives will be used if the Hessian is available in AIMMS, and that a limited-memory quasi-Newton approximation will be performed if the Hessian is not available. Note that the Hessian is not available in AIMMS if one of the constraints contains a call to an external function!

