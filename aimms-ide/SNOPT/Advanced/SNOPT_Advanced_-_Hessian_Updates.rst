.. _SNOPT_Advanced_-_Hessian_Updates:


Hessian Updates
===============



**Type**:	Integer	

**Range**:	{1..1000000}	

**Default**:	10	



This option determines the number of BFGS updates after which all but the diagonal elements of the accumulated updates (of the Hessian) are discarded and the updating process starts again. This only holds when 'Limited memory' is chosen for the option **Hessian Memory**  (which is also the case if the value of that option is 'Automatic' and the number of nonlinear variables is greater than 75).



Broadly speaking, the more updates stored, the better the quality of the approximate Hessian. However, the more vectors stored, the greater the cost of each QP iteration. The default value is likely to give a robust algorithm without significant expense, but faster convergence can sometimes be obtained with significantly fewer updates (i.e., 5).



**Note** 

*	Setting the value of this option to for instance 20 (in combination with 'Limited memory' for the option **Hessian Memory** ) has a same effect as setting the value of the option **Hessian Frequency**  equal to 20 (in combination with 'Full memory' for the **Hessian Memory** ), except that the first retains the current diagonal during resets.




**Learn more about** 

*	:ref:`SNOPT_Advanced_-_Hessian_Frequency`  
*	:ref:`SNOPT_Advanced_-_Hessian_Memory`  



