

.. _Options_NonlinPres_-_Presolve_remove_dupl_vars:


Presolve Remove Duplicate Variables
===================================



Type:	Selection	

Range:	The settings listed below	

Default:	On	



This option controls whether the AIMMS Presolver should remove duplicate variables. If two variables in a mathematical program have the same coefficient in the objective function(s) and in each constraint, then one of the variables is redundant and can be removed. Possible values are:



*	On
*	Off




For example, suppose that the variables X and Y have the same coefficient in every row of the mathematical program and the bounds are as follows: 


	


	-∞ ≤ X ≤ ∞


	 0 ≤ Y ≤ ∞





In this case, it is possible to fix the variable Y = 0, and remove it. 





**Note** 

*	Only duplicate variables are removed for which both upper bounds (or both lower bounds) are infinite.
*	Only duplicate linear variables are removed. 
*	This option has only an effect when solving a nonlinear model and the option **Nonlinear Presolve**  is switched on, or when solving a linear, quadratic or quadratically-constrained model and the option **Linear Presolve**  is switched on, or if the function GMP::Instance::CreatePresolved is used.




**Learn more about** 

*	:ref:`Options_NonlinPres_-_LinearPresolve` 
*	:ref:`Options_NonlinPres_-_NonlinearPresolve`  



