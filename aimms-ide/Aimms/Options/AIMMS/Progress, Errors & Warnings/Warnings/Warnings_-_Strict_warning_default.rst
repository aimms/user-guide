

.. _option-AIMMS-strict_warning_default:


Strict Warning Default
======================



:Type:	Selection
:Range:	The settings listed below	
:Default:	Off



This option provides the actual warning level for options that have option value ``strict warning default``.
This can be one of the following values:


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

*	:ref:`option-AIMMS-maximal_number_of_warnings_reported` 
*	:ref:`sec:exec.error`

