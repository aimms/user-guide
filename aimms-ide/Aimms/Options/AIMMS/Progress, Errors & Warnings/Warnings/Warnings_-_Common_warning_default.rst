

.. _Options_Warnings_-_Common_warning_default:


Common warning default
======================



Type:	Selection

Range:	The settings listed below	

Default:	Warning_handle



This option provides the actual warning level for options that have option value '``common warning default`` '. This can be one of the following values:






.. list-table::

   * - *	Off	
     - Do not issue a warning
   * - *	Warning_collect
     - Issue a warning and post it to the global error and warning collector
   * - *	Warning_handle
     - Issue a warning and post it to the nearest error handler
   * - *	Error
     - Issue an error
   * - *	Error_in_develop_else_warning
     - In a developer system same as Error, in a deployment system same as Warning_handle
   * - *	Error_in_develop_else_off
     - In a developer system same as Error, in a deployment system same as Off
   * - *	Warning_in_develop_else_off
     - In a developer system same as Warning_handle, in a deployment system same as Off






**Learn more about** 

*	:ref:`Options_Warnings_-_Maximal_Number_of_W` 
*	Search for Grouping warnings (Language reference)









