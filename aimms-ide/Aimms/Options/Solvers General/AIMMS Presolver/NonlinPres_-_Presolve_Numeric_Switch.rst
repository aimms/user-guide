

.. _Options_NonlinPres_-_Presolve_Numeric_Switch:


Presolve Numeric Switch
=======================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Automatic	



This option controls whether the AIMMS Presolver should focus on precision in numerically difficult problems, e.g., problems with large matrix coefficients or large (finite) variable bounds. Possible values are:



*	Off
*	Automatic
*	On




Focussing on precision might have a negative impact on the performance. At the default setting, AIMMS makes an automatic choice based on the matrix coefficients and variable bounds.




