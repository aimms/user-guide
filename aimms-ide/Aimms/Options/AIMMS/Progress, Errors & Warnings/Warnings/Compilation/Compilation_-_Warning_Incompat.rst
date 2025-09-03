

.. _option-AIMMS-warning_incompatible_argument_data_type:


Warning Incompatible Argument Data Type
=======================================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Common_warning_default	



This option determines what happens during compilation when there is call to a function or procedure with an argument of which the data type is incompatible with the data type of the argument as declared within the function or procedure. This situation is ignored, reported as a warning, or interpreted as an error, depending on the following settings:




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




An example of such a situation arises in the following model fragment, where the function "twice", of which the argument is declared as parameter, is called with a string parameter.



``STRING PARAMETER:`` 

``identifier : p`` 

``definition : "hello" ;`` 

``PARAMETER:`` 

``identifier : q`` 

``definition : twice(p) ;`` 

``FUNCTION`` 

``identifier : twice`` 

``arguments : a`` 

``PARAMETER:`` 

``identifier : a`` 

``property  : Input ;`` 

``body :`` 

``twice:=2*a;`` 

``ENDFUNCTION ;`` 



**Note** 

*	If you set this option to "Off" or "Warning", then the results of a mismatch in arguments are not predictable. You may use this in a call to an external procedure or function, as long as you know what you are doing.
*	With the option **Maximal Number of Warnings Reported** you can set the maximal number of warnings that are shown in errors/warnings and message window.




**Learn more about** 

*	:ref:`option-AIMMS-maximal_number_of_warnings_reported` 
*	:ref:`option-AIMMS-common_warning_default` 
*	:ref:`option-AIMMS-strict_warning_default` 
*	:ref:`option-AIMMS-communicate_warnings_to_end_users` 






