

.. _option-IPOPT-objective_function_scaling_factor:


Objective function scaling factor
=================================



:Type:	Floating point number	
:Range:	[-1e+019,1e+019]	
:Default:	1	



This option sets a scaling factor for the objective function. The scaling is seen internally by IPOPT but the unscaled objective is reported in the console output. If additional scaling parameters are computed (e.g., gradient-based), both factors are multiplied. If this value is chosen to be negative, IPOPT will maximize the objective function instead of minimizing it.



**Learn more about** 

*	:ref:`option-IPOPT-nlp_scaling_method` 
