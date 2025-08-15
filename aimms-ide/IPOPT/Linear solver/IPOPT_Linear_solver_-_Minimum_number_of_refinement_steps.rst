

.. _IPOPT_Linear_solver_-_Minimum_number_of_refinement_steps:


Minimum number of refinement steps
==================================



**Type**:	Integer	

**Range**:	{0..2147483647}	

**Default**:	1	



This option determines the minimum number of iterative refinement steps per linear system solve. Iterative refinement (on the full non-symmetric system) is performed for each right hand side. At least **Minimum Number of Refinement Steps**  iterative refinement steps are enforced per right hand side.



**Learn more about** 

*	:ref:`IPOPT_Linear_solver_-_Maximum_number_of_refinement_steps` 
