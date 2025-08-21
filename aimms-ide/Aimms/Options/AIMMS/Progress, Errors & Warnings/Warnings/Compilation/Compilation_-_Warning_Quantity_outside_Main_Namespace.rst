

.. _option-AIMMS-warning_quantity_outside_main_namespace:


Warning Quantity outside Main Namespace
=======================================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Warning in Develop else off		



It is recommended to declare all your quantities in the main model and not in Libraries or Modules. This assures that all units are easily accessible throughout the model.

If you are creating a (generic) library you can use the attribute Required Units to make sure that the main model will automatically create the required units.



*	Warning_in_develop_else_off
*	Error_in_develop_else_off
*	Off







**Learn more about** 

*	:ref:`option-AIMMS-maximal_number_of_warnings_reported` 
*	:ref:`option-AIMMS-communicate_warnings_to_end_users` 






