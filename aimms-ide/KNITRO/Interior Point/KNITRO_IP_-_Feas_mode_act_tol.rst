.. _KNITRO_IP_-_Feas_mode_act_tol:


Feasible Mode Activation Tolerance
==================================



:Type:	Floating point number	
:Range:	[0,1]	
:Default:	1e-4	



This option specifies the tolerance tol in



	cl + tol ≤ c(x) ≤ cu - tol



by which the iterate must be feasible with respect to the inequality constraints before the feasible mode becomes active. This option is only valid if the option **Feasible Mode**  is switched on.



**Note** 

*	This option can only be used with the interior-point optimizers.




**Learn more about** 

*	:ref:`KNITRO_IP_-_Feasible_mode`  



