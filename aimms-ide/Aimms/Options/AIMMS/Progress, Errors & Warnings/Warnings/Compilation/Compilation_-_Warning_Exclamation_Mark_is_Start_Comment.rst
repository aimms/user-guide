

.. _option-AIMMS-warning_exclamation_mark_equals_is_start_comment:


Warning Exclamation Mark Equals is Start Comment
================================================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Common_warning_default	



This option determines what happens in case AIMMS encounters the string "!=" in the model text:




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




Consider the following constraint:



CONSTRAINT:

  identifier  : someRestr

  index domain : (i,j) | i != j

  definition  : ...



In this constraint, the "!" in the index domain starts a comment, it is not part of the "not equal" operator as seen in some other computer languages. Thus AIMMS will issue the message: 

"Warning: An exclamation mark in AIMMS starts a comment; the operator "!=" is not supported but the operator "<>" is.", encouraging the constraint to be written as:





CONSTRAINT:

  identifier  : someRestr

  index domain : (i,j) | i <> j

  definition  : ...





**Note** 

*	With the option **Maximal Number of Warnings Reported** you can set the maximal number of warnings that are shown in errors/warnings and message window.




**Learn more about** 

*	:ref:`option-AIMMS-maximal_number_of_warnings_reported` 
*	:ref:`option-AIMMS-common_warning_default` 
*	:ref:`option-AIMMS-strict_warning_default` 
*	:ref:`option-AIMMS-communicate_warnings_to_end_users` 



