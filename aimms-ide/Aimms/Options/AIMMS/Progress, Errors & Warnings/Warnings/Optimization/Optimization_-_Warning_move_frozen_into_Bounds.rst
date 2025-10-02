

.. _option-AIMMS-warning_move_frozen_into_bounds:


Warning Move Frozen into Bounds
===============================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Common_warning_default	

This option determines what happens to the .level value of a frozen variable if this value is currently outside the bounds of the variable.
Only when set to Error the .level value will not be changed. For all other settings the .level value  will be changed to the value of the closest
bound, and an optional warning message is triggered.

This option is no longer valid for the new mathematical program generator. This new generator uses the option 'move_nonvar_level_within_bounds' and
will act according to that option without any error or warning message.

.. list-table::

   * - *	Off	
     - Do not issue a warning.
   * - *	Warning_collect
     - Issue a warning and post it to the global error and warning collector.
   * - *	Common_warning_default
     - Take action depending on the option 'Common warning default'.
   * - *	Warning_handle
     - Issue a warning and post it to the nearest error handler.
   * - *	Strict_warning_default
     - Take action depending on the option 'Strict warning default'.
   * - *	Error
     - Issue an error.
   * - *	Error_in_develop_else_warning
     - In a developer system same as Error, in a deployment system same as Warning_handle
   * - *	Error_in_develop_else_off
     - In a developer system same as Error, in a deployment system same as Off
   * - *	Warning_in_develop_else_off
     - In a developer system same as Warning_handle, in a deployment system same as Off


*	:ref:`option-AIMMS-move_nonvar_level_within_bounds` 
*	:ref:`option-AIMMS-common_warning_default` 
*	:ref:`option-AIMMS-strict_warning_default` 
*	:ref:`option-AIMMS-communicate_warnings_to_end_users` 

