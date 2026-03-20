

.. _option-IPOPT-acceptable_constraint_violation_tolerance:


Acceptable Constraint Violation Tolerance
=========================================



:Type:	Floating point number	
:Range:	[1e-010,1e+019]	
:Default:	0.01	



This option specifies the acceptable absolute tolerance on the constraint violation. "Acceptable" termination requires that the max-norm of the (unscaled) constraint violation is less than this threshold; see also the option **Acceptable Relative Convergence Tolerance**.



**Learn more about** 

*	:doc:`IPOPT_Termination_-_Acceptable_relative_convergence_tolerance` 
