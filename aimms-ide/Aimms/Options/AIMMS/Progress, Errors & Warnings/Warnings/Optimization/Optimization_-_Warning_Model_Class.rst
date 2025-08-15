

.. _Options_Optimization_-_Warning_Model_Class:


Warning Model Class
===================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Common_warning_default	



This option determines what happens when the type of mathematical program does not correspond to the model class, depending on the following settings:




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




For example, this situation arises when a linear model is declared as "nlp".



**Note** 

*	If this option is set to "Off" or "Warning", the mathematical program will be solved using the specified model class.
*	With the option Maximal Number of Warnings Reported you can set the maximal number of warnings that are shown in errors/warnings and message window.




**Learn more about** 

*	:ref:`Options_Warnings_-_Maximal_Number_of_W` 
*	:ref:`Model-Explorer_Creating_a_Mathematical_Progra` 
*	:ref:`Options_Warnings_-_Common_warning_default` 
*	:ref:`Options_Warnings_-_Strict_warning_default` 
*	:ref:`Options_Warnings_-_Communicate_warnings_to_end_users` 






