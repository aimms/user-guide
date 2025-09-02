

.. _option-AIMMS-warning_explicit_element_not_in_set:


Warning Explicit Element not in Set
===================================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Error	



This option determines what happens when a statement contains an explicit element name that is not in the associated set at the time the statement is executed.


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

.. code-block:: text

	Set Cities { 
	    Definition: data { Paris, London };
	}
	ElementParameter MyCity {
	    Range: Cities;
	}
	Procedure MainExecution {
	    Body: {
	        MyCity := 'Amsterdam';
	    }
	}


When executing procedure 'MainExecution', 'Amsterdam' is not an element of the set 'Cities' 


**Note** 

*	If the setting of this option does not result in Error, the element will be translated to an empty element.
*	With the option **Maximal Number of Warnings Reported** you can set the maximal number of warnings that are shown in errors/warnings and message window.


**Learn more about** 

*	:ref:`option-AIMMS-maximal_number_of_warnings_reported` 
*	:ref:`option-AIMMS-common_warning_default` 
*	:ref:`option-AIMMS-strict_warning_default` 
*	:ref:`option-AIMMS-communicate_warnings_to_end_users` 

