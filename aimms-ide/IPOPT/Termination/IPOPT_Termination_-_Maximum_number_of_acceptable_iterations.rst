

.. _IPOPT_Termination_-_Maximum_number_of_acceptable_iterations:


Maximum number of acceptable iterations
=======================================



**Type** :	Integer	

**Range** :	{0..2147483647}	

**Default** :	15	



This option sets the number of "acceptable" iterates before triggering termination. If the algorithm encounters this many successive "acceptable" iterates (see the option **Acceptable Relative Convergence Tolerance** ), it terminates, assuming that the problem has been solved to best possible accuracy given round-off. If it is set to 0, this heuristic is disabled.



**Learn more about** 

*	:ref:`IPOPT_Termination_-_Acceptable_relative_convergence_tolerance` 
