

.. _Options_Compilation_-_Warning_Round:


Warning Round
=============



Type:	Selection	

Range:	The settings listed below	

Default:	Common_warning_default



This option determines what happens whenever AIMMS expects an integral value, but a fractional one is provided. Consider the following example:



  p(i) := p(i + 1.5)



In that case AIMMS will issue the warning message: "The value 1.5 is too far (0.5) from its rounded value, see also the options warning_round and warning_round_tolerance."



The option "Warning_Round" determines what will happen when AIMMS expects an integral value, but a fractional one is provided, depending on the following settings:




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

*	Warning round tolerance is the tolerance used on integrality; if the absolute difference between a fractional value and its rounded value is less than this tolerance, then that value is considered to be integer.
*	With the option Maximal Number of Warnings Reported you can set the maximal number of warnings that are shown in errors/warnings and message window.




**Learn more about** 

*	:ref:`Options_Warnings_-_Maximal_Number_of_W` 
*	:ref:`Options_Warnings_-_Common_warning_default` 
*	:ref:`Options_Warnings_-_Strict_warning_default` 
*	:ref:`Options_Warnings_-_Communicate_warnings_to_end_users` 
*	:ref:`Options_Compilation_-_Warning_Round_Tolerance` 
