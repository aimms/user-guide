

.. _Options_NonlinPres_-_PresolvConstrUsed:


Presolve Constraints Used
=========================



**Type**:	Selection	

**Range**:	The settings listed below	

**Default**:	All	



This option controls the type of constraints that are used by the AIMMS Presolver to reduce the bounds of the variables (using Feasibility-Based Bound Tightening). Possible values are:



*	Linear
*	Nonlinear
*	All




The largest amount of reductions will be obtained if all constraints are used; however reducing the bounds of the variables by using nonlinear constraints might sometimes be time consuming.





**Note** 

*	This option has only an effect when solving a nonlinear model and the option **Nonlinear Presolve**  is switched on, or when solving a linear, quadratic or quadratically-constrained model and the option **Linear Presolve**  is switched on, or if the function GMP::Instance::CreatePresolved is used.




**Learn more about** 

*	:ref:`Options_NonlinPres_-_LinearPresolve` 
*	:ref:`Options_NonlinPres_-_NonlinearPresolve`  



