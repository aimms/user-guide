.. _GUROBI_General_-_Calculate_Kappa:


Calculate Kappa
===============



:Type:	Selection	
:Range:	The settings listed below	
:Default:	No	



This option can be used to display the basis condition number ('kappa'). The information will be printed in the message window. Possible values are:



*	No
*	Yes
*	Exact




The basis condition number can be used to measure the sensitivity of a linear problem to the problem data.





Setting 'Yes' calculates a quick estimate of the condition number. Setting 'Exact' computes the exact condition number which sometimes requires a substantial time.





The basis condition number will only be calculated for LP and RMIP models, and during the postsolve of a MIP model which can be enforced by switching on the general solvers option **MIP Calculate Sensitivity Information** .





**Learn more about** 

*	:ref:`Options_Postsolve_-_MIP_Calculate_Sensitivity_Info` 
