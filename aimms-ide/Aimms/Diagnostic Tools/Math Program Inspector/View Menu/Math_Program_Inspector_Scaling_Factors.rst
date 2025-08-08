

.. _Diagnostic-Tools_Math_Program_Inspector_Scaling_Factors:


Scaling Factors
===============

**Description** 

The Scaling Factors tab becomes only available after selecting the :ref:`Diagnostic-Tools_Math_Program_Inspector_Scale_Model`  action from the Actions menu. Note that this action is only available for linear models.



This tab shows the scaling factors of all variables in the model in the upper half and the scaling factors of all constraints in the model in the lower half. If you select a variable or constraint in the Scaling Factors tab, you can use right-mouse-click to open the attributes window of the corresponding variable or constraint.



If you want to use one of the calculated scaling factors in your model then you should update the Unit attribute in the attributes window of the corresponding variable or constraint. If the Unit attribute is empty then you can just fill in the scaling factor. If the Unit attribute contains an actual unit then you can change the unit or multiply it by the scaling factor. For example, if a variable has unit [kg] and the scaling factor is 1000 then you can change the unit to [1000*kg] but it would be better to use [ton].



**Learn more about** 

*	:ref:`Diagnostic-Tools_Math_Program_Inspector_Scale_Model` 
*	:ref:`sec:units.ident`



