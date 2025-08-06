

.. _IPOPT_Restoration_phase_-_Maximum_multipliers_infeasible_problem:


Maximum multipliers infeasible problem
======================================



**Type** :	Floating point number	

**Range** :	[1e-010,1e+019]	

**Default** :	1e+008	



This option sets the multiplier threshold for activating the **Quickly Detect Infeasible Problem**  option. If the max norm of the constraint multipliers becomes larger than this value and option **Quickly Detect Infeasible Problem**  is switched on, then the restoration phase is entered.



**Learn more about** 

*	:ref:`IPOPT_Restoration_phase_-_Quickly_detect_infeasible_problem` 
