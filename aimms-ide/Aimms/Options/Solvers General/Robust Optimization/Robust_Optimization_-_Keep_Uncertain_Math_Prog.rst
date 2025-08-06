

.. _Options_Robust_Optimization_-_Keep_Uncertain_Math_Prog:


Keep Uncertain Mathematical Program
===================================



Type:	Selection	

Range:	The settings listed below	

Default:	Off	



The robust counterpart for a symbolic mathematical program with uncertain data is generated using the procedure GMP::Instance::GenerateRobustCounterpart. To do so, AIMMS first collects all symbolic information to generate an intermediate GMP in which all uncertain parameters are treated as variables. This uncertain mathematical program might contain quadratic constraints in case uncertain parameters are multiplied by variables, or if the model contains ellipsoidal uncertainty constraints. The generated uncertain mathematical program is then used to construct the robust counterpart GMP.



Normally there is no use for keeping this uncertain mathematical program and therefore it is deleted to save memory. By switching on this option, the uncertain mathematical program will be kept by AIMMS. It will be deleted if the corresponding robust counterpart GMP is deleted.



Possible values are:



*	On
*	Off




If you want to use the procedure GMP::Robust::EvaluateAdjustableVariables to evaluate adjustable variables, this option must be switched on.





**Note** 

*	If this option is switched on then the memory used by AIMMS might increase significantly.
