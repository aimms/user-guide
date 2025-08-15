.. _KNITRO_General_-_Honor_Bounds:


Honor Bounds
============



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Only for initial point	



This option determines whether or not Knitro should enforce satisfaction of simple variable bounds throughout the optimization. By default, Knitro does not require that the bounds on the variables are satisfied at intermediate iterates. If this option is switched to 'Always' then Knitro enforces that the initial point and all subsequent solution estimates satisfy the bounds on the variables. Possible values are:



*	Never
*	Always
*	Only for initial point




This option might be switched to 'Always' if the objective function or a nonlinear constraint function is undefined at points outside the bounds.





**Learn more about** 

*	:ref:`KNITRO_IP_-_Feasible_mode`  
