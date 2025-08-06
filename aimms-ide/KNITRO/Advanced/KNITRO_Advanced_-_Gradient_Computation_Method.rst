.. _KNITRO_Advanced_-_Gradient_Computation_Method:


Gradient Computation Method
===========================



**Type** :	Selection	

**Range** :	The settings listed below	

**Default** :	AIMMS computes	



This option specifies how to compute the gradients of the objective and constraint functions. By default AIMMS will compute the gradients. Only in some rare situations the setting of this option should be changed. Possible values are:



*	AIMMS computes
*	Forward finite-differences
*	Central finite-differences




Using first derivative approximations may seriously degrade the performance of Knitro and the likelihood of converging to a solution. The centered finite-difference approximation is often more accurate than the forward finite-difference approximation; however, it is more expensive to compute if the cost of evaluating a function is high.




