.. _KNITRO_Presolve_-_Presolve_Substitution_Tolerance:


Presolve Substitution Tolerance
===============================



:Type:	Floating point number	
:Range:	[0,1e20]	
:Default:	1e-2	



This option determines the tolerance used by the Knitro presolver for performing a variable substitution. This is a relative tolerance on coefficients involved with the substituted variable. Higher values mean that less reductions will be applied (potentially improving numerical focus). Zero value means all possible substitutions are applied. 



**Learn more about** 

*	:ref:`KNITRO_Presolve_-_Presolve`  
*	:ref:`KNITRO_Presolve_-_Presolve_Substitution`  
