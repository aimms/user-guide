

.. _Options_Math_Program_Inspector_-_Store:


Store Complete Solver Solution
==============================



**Type**:	Selection	

**Range**:	The settings listed below	

**Default**:	No	



This option determines whether AIMMS will store the complete solver solution after a solve. This includes the basis statuses, constraint level values and the marginal values, regardless of the setting of the following options:



*	:ref:`Options_Sensitivity_-_Always_Store_Bas`  
*	:ref:`Options_Sensitivity_-_Always_Store_Con`  
*	:ref:`Options_Sensitivity_-_Always_Store_Mar`  




If this option is set to on, the Math Program Inspector has this information available and it will be shown. However, to store the basis statuses and the marginal values for MIP problems, AIMMS has to perform a postsolve step and therefore the following postsolve options should not be switched off:




*	:ref:`Options_Postsolve_-_MIP_Calculate_Sensitivity_Info`  
*	:ref:`Options_Postsolve_-_Postsolve`  




Possible values are:




*	No
*	Yes




**Note** 

*	For larger models, it takes time and memory to store this information, so this option should only be set if you are going to inspect the model in the Math Program Inspector. 
*	If the basic information and the marginal values are not stored for all variables and constraints in a MIP problem, then the degeneracy information will not be available in the Math Program Inspector.




**Learn more about** 

*	:ref:`Diagnostic-Tools_AIMMS_Math_Program_Inspector` 



