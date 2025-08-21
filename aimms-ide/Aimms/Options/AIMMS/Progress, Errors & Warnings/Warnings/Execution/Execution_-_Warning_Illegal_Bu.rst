

.. _option-AIMMS-warning_illegal_bulk_mode_write:


Warning Illegal Bulk Mode Write
===============================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Strict_warning_default	



This options specifies the behavior of AIMMS in case a bulk write statement is executed and the underlying data source doesn't support this mode. Possible values are:



This situation is ignored, reported as a warning, or interpreted as an error, depending on the following settings:




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

*	If you set this option to "Off" or "Warning", AIMMS will try to use an alternative writing mode if the data source does not support bulk write.
*	With the option Maximal Number of Warnings Reported you can set the maximal number of warnings that are shown in errors/warnings and message window.




**Learn more about** 

*	:ref:`option-AIMMS-maximal_number_of_warnings_reported` 
*	:ref:`Options_Warnings_-_Common_warning_default` 
*	:ref:`Options_Warnings_-_Strict_warning_default` 
*	:ref:`option-AIMMS-communicate_warnings_to_end_users` 



