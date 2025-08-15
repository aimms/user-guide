

.. _Options_Execution_-_Waning_empty_iterative_domain:


Warning_empty_iterative_domain
==============================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Error_in_develop_else_off	



For some iterative operators, for example Mean, the expression cannot be correctly evaluated if there are no elements in the iterative domain.






.. list-table::

   * - *	Off	
     - Do not issue a warning. The result is set to 0.0.
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




An example of such a situation arises when executing the following model:



``Set Cities {`` 

``index : c ;`` 

``definition : data{Paris,London} ;`` 

``}`` 

``Parameter selectedCities {`` 

``IndexDomain : c;`` 

``}`` 

``Parameter population {`` 

``IndexDomain : c;`` 

``}`` 

``Parameter result;`` 

``Procedure MainExecution {`` 

``body : {`` 

		``result := Mean( c | selectedCities(c), population(c));`` 

	``}`` 

``}`` 



When executing procedure 'MainExecution', if the parameter 'selectedCities' is empty the statement cannot calculate a valid Mean.



**Note** 

*	With the option Maximal Number of Warnings Reported you can set the maximal number of warnings that are shown in errors/warnings and message window.




**Learn more about** 

*	:ref:`Options_Warnings_-_Maximal_Number_of_W` 
*	:ref:`Options_Warnings_-_Common_warning_default` 
*	:ref:`Options_Warnings_-_Strict_warning_default` 
*	:ref:`Options_Warnings_-_Communicate_warnings_to_end_users` 






