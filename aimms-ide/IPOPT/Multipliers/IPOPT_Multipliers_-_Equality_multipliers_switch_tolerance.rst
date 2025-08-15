

.. _IPOPT_Multipliers_-_Equality_multipliers_switch_tolerance:


Equality multipliers switch tolerance
=====================================



**Type**:	Floating point number	

**Range**:	[0,1e+019]	

**Default**:	10	



This option specifies the tolerance for switching to full equality multiplier steps. This is only relevant if 'Primal and full' or 'Dual and full' is chosen for the option **Constraint Multipliers Step Size Method** . The step size for the equality constraint multipliers is taken to be one if the max-norm of the step size is less than this tolerance.



**Learn more about** 

*	:ref:`IPOPT_Multipliers_-_Constraint_multipliers_step_size_method` 
