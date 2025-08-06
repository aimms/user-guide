

.. _IPOPT_Termination_-_Acceptable_objective_change_tolerance:


Acceptable objective change tolerance
=====================================



**Type** :	Floating point number	

**Range** :	[0,1e+019]	

**Default** :	1e+019	



``This option specifies the "acceptance" stopping criterion based on objective function change. If the relative change of the objective function (scaled by Max(1,|f(x)|)) is less than this value, this part of the acceptable tolerance termination is satisfied; see also the option`` **Acceptable Relative Convergence Tolerance** . This is useful for the quasi-Newton option, which has trouble to bring down the dual infeasibility.



**Learn more about** 

*	:ref:`IPOPT_Termination_-_Acceptable_relative_convergence_tolerance` 
