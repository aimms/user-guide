

.. _Options_Math_Program_Inspector_-_Scale_using_Solution:


Scale Using Solution
====================



**Type**:	Selection	

**Range**:	The settings listed below	

**Default**:	No	



This option determines whether the scaling tool in the Math Program Inspector will use the current solution (if any) in the Math Program Inspector. Possible values are:



*	No
*	Yes




The scaling tool can be enabled by selecting the :ref:`Diagnostic-Tools_Math_Program_Inspector_Scale_Model`  action from the Actions menu in the Math Program Inspector. Please note that this action is only available for linear models.





By switching on this option the scaling tool will use the current solution (if any) in the Math Program Inspector to scale the model. The focus then (partially) shifts from scaling the coefficients, right-hand-side values and variable bounds, such that they become as close to 1 (in absolute sense) as possible, to obtaining a solution in which the variables have level values close to 1 (in absolute sense).





**Learn more about** 

*	:ref:`Diagnostic-Tools_AIMMS_Math_Program_Inspector` 
*	:ref:`Diagnostic-Tools_Math_Program_Inspector_Scale_Model` 



