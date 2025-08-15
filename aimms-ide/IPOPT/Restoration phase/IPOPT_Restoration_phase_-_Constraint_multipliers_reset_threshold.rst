

.. _IPOPT_Restoration_phase_-_Constraint_multipliers_reset_threshold:


Constraint multipliers reset threshold
======================================



:Type:	Floating point number	
:Range:	[0,1e+019]	
:Default:	0	



This option determines the threshold for resetting equality and inequality multipliers after the restoration phase. After returning from the restoration phase, the constraint multipliers are recomputed by a least square estimate. This option triggers when those least-square estimates should be ignored.

