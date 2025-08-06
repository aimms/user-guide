.. _SNOPT_SQP_-_DerivativeOption:


Derivative Option
=================



**Type** :	Selection	

**Range** :	The settings listed below	

**Default** :	All gradients are known	



This option specifies which nonlinear function gradients are known analytically and will be supplied to SNOPT by AIMMS. If the value of this option equals 'Some gradients are unknown' then some components of the objective gradient are unknown and some of the constraint gradients are unknown. This situation might occur if you use an external function in one of the constraints. If the value equals 'All gradients are known' (the default) then all objective and constraint gradients are known.



The default value should be used whenever possible. It is the most reliable and will usually be the most efficient.



If the value is 'Some gradients are unknown' SNOPT will estimate the missing components of G(x) using finite differences. This could increase the total run-time substantially, and there is less assurance that an acceptable solution will be located. If the nonlinear variables are not well scaled, it may be necessary to specify a nonstandard value for the option **Difference Interval** .



Possible values are:



*	Some gradients are unknown
*	All gradients are known




**Learn more about** 

*	:ref:`SNOPT_SQP_-_DifferenceInterval`  
