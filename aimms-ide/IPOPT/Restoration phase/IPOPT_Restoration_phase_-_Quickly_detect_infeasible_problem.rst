

.. _IPOPT_Restoration_phase_-_Quickly_detect_infeasible_problem:

Quickly detect infeasible problem
=================================



**Type**:	Selection	

**Range**:	The settings listed below	

**Default**:	No	



This option can be used to enable heuristics to quickly detect an infeasible problem. This option is meant to activate heuristics that may speed up the infeasibility determination if you expect that there is a good chance for the problem to be infeasible. In the filter line search procedure, the restoration phase is called more quickly than usually, and more reduction in the constraint violation is enforced before the restoration phase is left. If the problem is square, this option is enabled automatically. Possible values are:



*	No
*	Yes




**Learn more about** 

*	:ref:`IPOPT_Restoration_phase_-_Maximum_multipliers_infeasible_problem` 
*	:ref:`IPOPT_Restoration_phase_-_Minimum_violation_infeasible_problem` 
