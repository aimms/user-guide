.. _SNOPT_Advanced_-_Hessian_Frequency:


Hessian Frequency
=================



**Type**:	Integer	

**Range**:	{1..1000000}	

**Default**:	999999	



This option determines the number of BFGS updates after which the Hessian approximation is reset to the identity matrix. This only holds when 'Full memory' is chosen for the option **Hessian Memory**  (which is also the case if the value of that option is 'Automatic' and the number of nonlinear variables is less than or equal to 75). (For certain problems, occasional resets may improve convergence, but in general they should not be necessary.)



**Note** 

*	Setting the value of this option to for instance 20 (in combination with 'Full memory' for the option **Hessian Memory** ) has a same effect as setting the value of the option **Hessian Updates**  equal to 20 (in combination with 'Limited memory' for the **Hessian Memory** ), except that the latter retains the current diagonal during resets.




**Learn more about** 

*	:ref:`SNOPT_Advanced_-_Hessian_Memory`  
*	:ref:`SNOPT_Advanced_-_Hessian_Updates`  



