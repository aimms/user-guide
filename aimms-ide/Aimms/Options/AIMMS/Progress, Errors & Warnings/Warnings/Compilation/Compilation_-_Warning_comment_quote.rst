

.. _option-AIMMS-warning_comment_quote:


Warning Comment Quote
=====================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Off	



In general, the commentary text in the model does not have to obey to a specific syntax. However, when renaming identifiers
throughout your model, AIMMS also searches for identifier references between single quotes in a commentary text.

With this option, you can let AIMMS detect a mismatch in quotes in a comment text during compilation (i.e. one or more single
quotes that do not properly include an identifier name). By default, this situation is ignored, but you can let AIMMS generate
a warning or error. Possible values for this option are:


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

