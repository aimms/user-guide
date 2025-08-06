.. _CONOPT_Advanced_-_Steplength_Multiplier:


Steplength Multiplier
=====================



**Type** :	Floating point number	

**Range** :	[2,100]	

**Default** :	4	



The step length in the one-dimensional line search is not allowed to increase by a factor of more than **Steplength Multiplier**  between steps for models with nonlinear constraints and by a factor of more than 100 * **Steplength Multiplier**  for models with linear constraints.



