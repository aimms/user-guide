

.. _IPOPT_Multipliers_-_Constraint_multipliers_step_size_method:


Constraint multipliers step size method
=======================================



**Type**:	Selection	

**Range**:	The settings listed below	

**Default**:	Primal	



This option determines how the step size will be calculated when updating the constraint multipliers. Possible values are:



*	Primal
*	Bound multipliers
*	Minimum of primal and bound multipliers
*	Maximum of primal and bound multipliers
*	Full
*	Min dual infeasibility
*	Safer min dual infeasibility
*	Primal and full
*	Dual and full
*	Acceptor




Setting 'Bound multipliers' is good for LPs.





Setting 'Full' implies taking a full step of size one.





Setting 'Min dual infeasibility' implies choosing the step size minimizing new dual infeasibility; setting 'Safer min dual infeasibility' is the same but with a safeguard.





Setting 'Primal and full' means: use the primal step size, and the full step if the step size is smaller than or equal to the value of the option **Equality Multipliers Switch Tolerance** .





Setting 'Dual and full' means: use the dual step size, and the full step if the step size is smaller than or equal to the value of the option **Equality Multipliers Switch Tolerance** .





Setting 'Acceptor' calls LSAcceptor to get the step size.





**Learn more about** 

*	:ref:`IPOPT_Multipliers_-_Equality_multipliers_switch_tolerance` 
