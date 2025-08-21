.. _option-KNITRO-tighten_variable_bounds:


Tighten Variable Bounds
=======================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Automatic	



This option determines whether or not to enable the Knitro presolve operation to tighten variable bounds. Possible values are:



*	Automatic
*	Off
*	On




At setting 'Automatic' Knitro decides, which may depend on the algorithm.





At setting 'Off' variable bounds are tightened, unless it removes a constraint.





**Learn more about** 

*	:ref:`option-KNITRO-presolve`  
