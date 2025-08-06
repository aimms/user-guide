

.. _IPOPT_Restoration_phase_-_Bound_multipliers_reset_threshold:


Bound multipliers reset threshold
=================================



**Type** :	Floating point number	

**Range** :	[0,1e+019]	

**Default** :	1000	



This option determines the threshold for resetting bound multipliers after the restoration phase. After returning from the restoration phase, the bound multipliers are updated with a Newton step for complementarity. Here, the change in the primal variables during the entire restoration phase is taken to be the corresponding primal Newton step. However, if after the update the largest bound multiplier exceeds the threshold specified by this option, the multipliers are all reset to 1.

