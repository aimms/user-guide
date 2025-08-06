

.. _IPOPT_Termination_-_Acceptable_complementarity_tolerance:


Acceptable complementarity tolerance
====================================



**Type** :	Floating point number	

**Range** :	[1e-010,1e+019]	

**Default** :	0.01	



This option specifies the acceptable absolute tolerance on the complementarity. "Acceptable" termination requires that the max-norm of the (unscaled) complementarity is less than this threshold; see also the option **Acceptable Relative Convergence Tolerance** .



**Learn more about** 

*	:ref:`IPOPT_Termination_-_Acceptable_relative_convergence_tolerance` 
