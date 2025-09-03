

.. _option-AIMMS-warning_repeated_iterative_evaluation:


Warning Repeated Iterative Evaluation
=====================================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Strict_warning_default	



This option determines what happens during compilation when an iterative operator doesn't depend on some of the indices and subsequently executing the encompassing statement will result in repeatedly evaluating the iterative operator to the same result.



Consider the example:



	``a(i) := sum(j,b(j));`` 



In this example the result of ``sum(j,b(j))``  doesn't depend on ``i`` , and this summation will therefore be repeatedly evaluated with the same result for every ``i`` .



This will be ignored, reported as a warning, or interpreted as an error, depending on the following settings:




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






