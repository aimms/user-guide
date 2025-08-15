.. _SNOPT_Advanced_-_Hessian_Memory:


Hessian Memory
==============



**Type**:	Selection	

**Range**:	The settings listed below	

**Default**:	Automatic	



This option selects the method for storing and updating the approximate Hessian. (SNOPT uses a quasi-Newton approximation to the Hessian of the Lagrangian. A BFGS update is applied after each major iteration.)



If 'Full memory' is chosen, the approximate Hessian is treated as a dense matrix and the BFGS updates are applied explicitly. This setting is most efficient when the number of nonlinear variables is not too large (less than 75). In that case, the storage requirement is fixed and one can expect 1-step Q-superlinear convergence to the solution.



The setting 'Limited memory' should be used on problems where the number of nonlinear variables is very large. In that case a limited-memory procedure is used to update a diagonal Hessian approximation, Hr, a limited number of times. (Updates are accumulated as a list of vector pairs. They are discarded at regular intervals after Hr has been reset to their diagonal.)



The default setting 'Automatic' means that full memory is chosen when the number of nonlinear variables is smaller than or equal to 75, and limited memory else.



Possible values are:



*	Automatic
*	Full memory
*	Limited memory




**Learn more about** 

*	:ref:`SNOPT_Advanced_-_Hessian_Frequency`  
*	:ref:`SNOPT_Advanced_-_Hessian_Updates`  



