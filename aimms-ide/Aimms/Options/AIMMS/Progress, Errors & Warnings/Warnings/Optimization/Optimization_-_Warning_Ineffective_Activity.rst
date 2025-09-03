

.. _option-AIMMS-warning_ineffective_activity:


Warning Ineffective Activity
============================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Common_warning_default



For parallel resources, it is checked whether each activity mentioned in the attribute "activities" is also referenced in one of the level modification attributes "level change", "begin change", and "end change".

Consider the following example:



.. code-block:: aimms

    Resource res {
        Usage: parallel;
        ScheduleDomain: Timeline;
        Activities: act1, act2, act3, act4;
        LevelRange: {
            {0..10}
        }
        LevelChange: act1: 1;
        BeginChange: act2: 2;
        EndChange: act3: 3;
    }


For this resource AIMMS will issue the message:

.. code-block:: text

    Warning: The activity act4, referenced in the activity attribute of res, is not referenced in any of the
    level modification attributes of that parallel schedule.


The option ``Warning_Ineffective_Activity`` determines how nonbinding global constraints are reported, depending on the following settings:


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

*	With the option **Maximal Number of Warnings Reported** you can set the maximal number of warnings that are shown in errors/warnings and message window.


**Learn more about** 

*	:ref:`option-AIMMS-maximal_number_of_warnings_reported` 
*	:ref:`option-AIMMS-common_warning_default` 
*	:ref:`option-AIMMS-strict_warning_default` 
*	:ref:`option-AIMMS-communicate_warnings_to_end_users` 
*	:ref:`option-AIMMS-warning_referenced_activities` 

