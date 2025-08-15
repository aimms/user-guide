

.. _IPOPT_Restoration_phase_-_Minimum_violation_infeasible_problem:


Minimum violation infeasible problem
====================================



**Type**:	Floating point number	

**Range**:	[0,1e+019]	

**Default**:	0.001	



This option sets the threshold for disabling **Quickly Detect Infeasible Problem**  option. If the constraint violation becomes smaller than this threshold, the heuristics in the filter line search used when option **Quickly Detect Infeasible Problem**  is switched on, are disabled. If the problem is square, this option is set to 0.



**Learn more about** 

*	:ref:`IPOPT_Restoration_phase_-_Quickly_detect_infeasible_problem` 
