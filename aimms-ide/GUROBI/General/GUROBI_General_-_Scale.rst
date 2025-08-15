.. _GUROBI_General_-_Scale:


Scale
=====



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Automatic	



This option enables or disables model scaling. Possible values are:



*	Automatic
*	Off
*	Equilibrium scaling
*	Geometric scaling
*	Multi-pass equilibrium scaling




By default, the rows and columns of the model are scaled in order to improve the numerical properties of the constraint matrix. The scaling is removed before the final solution is returned. Scaling typically reduces solution times, but it may lead to larger constraint violations in the original, unscaled model. Turning off scaling can sometimes produce smaller constraint violations. Choosing a different scaling option can sometimes improve performance for particularly numerically difficult models.





Setting 'Geometric scaling' is especially well suited for models with a wide range of coefficients in the constraint matrix rows or columns.





Settings 'Equilibrium scaling' and 'Multi-pass equilibrium scaling' are not as directly connected to any specific model characteristics, so experimentation with both settings may be needed to assess performance impact.




