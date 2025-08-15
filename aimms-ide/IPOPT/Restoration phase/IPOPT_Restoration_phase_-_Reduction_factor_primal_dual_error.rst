

.. _IPOPT_Restoration_phase_-_Reduction_factor_primal_dual_error:


Reduction factor primal dual error
==================================



:Type:	Floating point number	
:Range:	[0,1e+019]	
:Default:	0.9999	



This option specifies the required reduction in primal-dual error in the soft restoration phase. The soft restoration phase attempts to reduce the primal-dual error with regular steps. If the damped primal-dual step (damped only to satisfy the fraction-to-the-boundary rule) is not decreasing the primal-dual error by at least this factor, then the regular restoration phase is called. Choosing 0 here disables the soft restoration phase.

