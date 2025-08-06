

.. _Options_Optimization_-_Warning_Ineffective_Activity:


Warning Ineffective Activity
============================



Type:	Selection	

Range:	The settings listed below	

Default:	Common_warning_default



For parallel resources, it is checked whether each activity mentioned in the attribute "activities" is also referenced in one of the level modification attributes "level change", "begin change", and "end change".

Consider the following example:



RESOURCE:

  identifier   : res

  usage      : parallel

  schedule domain : Timeline

  activities   : act1, act2, act3, act4

  level range   : {0..10}

  level change  : act1: 1

  begin change  : act2: 2

  end change   : act3: 3



For this resource AIMMS will issue the message: "Warning: The activity act4, referenced in the activity attribute of res, is not referenced in any of the level modification attributes of that parallel schedule."



The option "``Warning_Ineffective_Activity`` " determines how nonbinding global constraints are reported, depending on the following settings:




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
*	:ref:`Options_Optimization_-_Warning_Referenced_Activities` 



