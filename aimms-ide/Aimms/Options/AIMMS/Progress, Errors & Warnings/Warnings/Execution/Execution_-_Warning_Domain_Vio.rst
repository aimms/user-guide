

.. _Options_Execution_-_Warning_Domain_Vio:


Warning Domain Violation
========================



Type:	Selection	

Range:	The settings listed below	

Default:	Error	



This option determines what happens when domains are violated, depending on the following settings:




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




An example of such a situation arises when executing the following model:



``SET:`` 

``identifier : Cities`` 

``definition : data{Paris,London} ;`` 

``SET:`` 

``identifier : FrenchCities`` 

``subset of : Cities;`` 

``PROCEDURE`` 

``identifier : MainExecution`` 

``body :`` 

``FrenchCities:={Paris,Toulouse};`` 

``ENDPROCEDURE ;`` 



When executing procedure 'MainExecution', there is a domain violation, because 'Toulouse' is not an element of the set 'Cities'.



**Note** 

*	If you set this option to "Off" or "Warning", data will be assigned to elements that are outside the domain.
*	With the option Maximal Number of Warnings Reported you can set the maximal number of warnings that are shown in errors/warnings and message window.




**Learn more about** 

*	:ref:`Options_Warnings_-_Maximal_Number_of_W` 
*	:ref:`Options_Warnings_-_Common_warning_default` 
*	:ref:`Options_Warnings_-_Strict_warning_default` 
*	:ref:`Options_Warnings_-_Communicate_warnings_to_end_users` 






