

.. _option-AIMMS-warning_variable_range_violation:


Warning Variable Range Violation
================================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Common_warning_default	



This option determines what happens during execution, when the numerical range of a variable is violated, depending on the following settings:


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


**Note** 

*	The setting of this option has effect on both numerical range violations in AIMMS code and in the graphical user interface.
*	The setting of this option has also an effect on the empty statement; because an empty statement is viewed as setting all elements to its default. You may consider moving the default inside the bounds.
*	With the option **Maximal Number of Warnings Reported** you can set the maximal number of warnings that are shown in errors/warnings and message window.


**Learn more about** 

*	:ref:`option-AIMMS-maximal_number_of_warnings_reported` 
*	:ref:`option-AIMMS-common_warning_default` 
*	:ref:`option-AIMMS-strict_warning_default` 
*	:ref:`option-AIMMS-communicate_warnings_to_end_users` 

