

.. _option-AIMMS-warning_stochastic_programming_scenario_consistency:


Warning Stochastic Programming Scenario Consistency
===================================================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Common_warning_default	



This option determines whether a consistency check on the scenarios in a stochastic program is executed.
In all but the last stage, for coefficients in a group of rows differing only in their scenario index,
the coefficients in a column with the same representative scenario should be the same. Whether the consistency
check is executed and whether a warning or error is given when the check fails depends on the following settings:


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
*	`Stochastic Programming <https://documentation.aimms.com/language-reference/optimization-modeling-components/stochastic-programming/index.html>`_

