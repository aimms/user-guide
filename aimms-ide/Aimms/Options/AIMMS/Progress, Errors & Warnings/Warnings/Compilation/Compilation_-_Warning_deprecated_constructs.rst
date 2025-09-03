

.. _option-AIMMS-warning_deprecated_constructs:


Warning Deprecated Constructs
=============================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Error_in_develop_else_off



The AIMMS syntax has not been completely the same over all the years it exists. To remain backward compatible with older models, the current compiler still accepts constructs that officially are not correct according to the syntax as described in the Language Reference. In future versions of the compiler (and execution system) some of these old syntax constructs will no longer be supported.

To make the developer aware of these constructs, the compiler will now give errors on it.

It is recommended to fix these errors, such that your model remains in sync with future AIMMS versions.



Possible values for this option are:




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



