

.. _Options_Compilation_-_Warning_Adapting:


Warning Adapting Range For Loop
===============================



Type:	Selection	

Range:	The settings listed below	

Default:	Common_warning_default	



This options determines what AIMMS will do when the range of a for loop is adapted within the for loop. This can be ignored, communicated via the message window as a warning to the user, or can result in a compilation error, corresponding to following settings:






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

*	With the option Maximal Number of Warnings Reported you can set the maximal number of warnings that are shown in errors/warnings and message window.




**Remark** 


When this option doesn't issue an error AIMMS will still try to execute the for loop. The number of times the loop is executed is however undefined and may vary between different AIMMS releases due to small changes.





**Learn more about** 

*	:ref:`Options_Warnings_-_Maximal_Number_of_W` 
*	:ref:`Options_Warnings_-_Common_warning_default` 
*	:ref:`Options_Warnings_-_Strict_warning_default` 
*	:ref:`Options_Warnings_-_Communicate_warnings_to_end_users` 






