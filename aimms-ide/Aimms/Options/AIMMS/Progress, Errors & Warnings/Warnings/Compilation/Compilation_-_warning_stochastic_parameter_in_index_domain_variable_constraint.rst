

.. _Options_Compilation_-_warning_stochastic_parameter_in_index_domain_variable_constraint:


Warning Stochastic Parameter in Index Domain Variable Constraint
================================================================



Type:	Selection	

Range:	The settings listed below	

Default:	Strict_warning_default	



AIMMS now warns when a stochastic parameter is used in the index domain of a variable or of a constraint. 



This warning is issued because AIMMS generates the stochastic mathematical program for only one scenario. In order to be able to present the full stochastic mathematical program it stores the differences with respect to the other scenarios. This is usually equivalent to generating all scenarios, except when the index domain of a variable / constraint contains references to stochastic parameters. This situation is ignored, reported as a warning, or interpreted as an error, depending on the following settings:




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




**Learn more about** 

*	:ref:`Options_Warnings_-_Maximal_Number_of_W`  
*	:ref:`Options_Warnings_-_Common_warning_default` 
*	:ref:`Options_Warnings_-_Strict_warning_default` 
*	:ref:`Options_Warnings_-_Communicate_warnings_to_end_users` 



