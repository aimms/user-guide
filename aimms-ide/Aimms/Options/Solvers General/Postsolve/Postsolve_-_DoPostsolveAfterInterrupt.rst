

.. _Options_Postsolve_-_DoPostsolveAfterInterrupt:


Do Postsolve after Interrupt
============================



Type:	Selection	

Range:	The settings listed below	

Default:	Off	



This option specifies whether or not the postsolve step will be skipped after a user interrupt or when the iteration or time limit is exceeded.



If this option is set to 'Off' (the default) then no postsolve will be done, i.e., the value of the option **Postsolve**  is treated as 'Off''. If the value of this option is set to 'On', then a postsolve will be done according to the setting of the options **Postsolve** , **Postsolve Continuous Variables** , **Postsolve Integer Variables**  and **MIP Calculate Sensitivity Information** . Note that the postsolve step itself cannot be interrupted.



Possible values of this option are:



*	On
*	Off




**Note** 

*	Please check the option **Postsolve**  for more information regarding the postsolve step.
*	In rare situations, namely if a MIP solve is interrupted before the root node LP is solved, an incumbent solution found by CPLEX might not be optimal regarding the continuous variables. If the postsolve step rounds and fixes the integer variables to solve the resulting LP problem then a solution with a better objective value might be found.




**Learn more about** 

*	:ref:`Options_Postsolve_-_MIP_Calculate_Sensitivity_Info`  
*	:ref:`Options_Postsolve_-_Postsolve` 
*	:ref:`Options_Postsolve_-_Postsolve_Continuous_Variables` 
*	:ref:`Options_Postsolve_-_Postsolve_Integer_Variables` 



