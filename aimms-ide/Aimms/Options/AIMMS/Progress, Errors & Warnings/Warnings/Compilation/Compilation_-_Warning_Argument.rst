

.. _option-AIMMS-warning_argument_defaults_mismatch:


Warning Argument Defaults Mismatch
==================================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Common_warning_default	



This option determines what AIMMS will do when a mismatch between the defaults of an actual and a formal argument of
a procedure is encountered during compilation. This can be ignored, communicated via the Message Window as a warning
to the user, or can result in a compilation error, corresponding to following settings:


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

*	If you choose not to report this situation as an error, AIMMS will try to retain the values (default or non-default) of each element when passing it back and forth to a procedure. For example, consider a parameter P with a default of 1.0, and pass it to a procedure with an output argument A that has a default of 2.0. If you empty the output parameter A within the body of the procedure, then on return from the procedure, the parameter P will be filled with the non-default value 2.0.
*	With the option **Maximal Number of Warnings Reported** you can set the maximal number of warnings that are shown in errors/warnings and message window.


**Learn more about** 

*	:ref:`option-AIMMS-maximal_number_of_warnings_reported` 
*	:ref:`option-AIMMS-common_warning_default` 
*	:ref:`option-AIMMS-strict_warning_default` 
*	:ref:`option-AIMMS-communicate_warnings_to_end_users` 

