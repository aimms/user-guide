

.. _Options_Compilation_-_Warning_Difference_Scalar_Reference_Substitution:


Warning Difference Scalar Suffix Reference Substitution
=======================================================



**Type**:	Selection	

**Range**:	The settings listed below	

**Default**:	Strict_warning_default	



Consider the following declarations:



  PARAMETER:

    identifier  : x_lo 

    initial data : 1 ;



  PARAMETER:

    identifier  : x_up 

    initial data : 5 ;



  PARAMETER:

    identifier  : x_mid ;



  VARIABLE:

    identifier  : x_scalar

    range    : [x_lo, x_up] ;



With these declarations the statement:



    x_mid := ( x_scalar.lower + x_scalar.upper ) / 2 ;



Will now give a different result:



   Up to and including 3.9.5/3.10.FR3:   	x_mid = 0

   3.9.6/3.10.PR1/3.11.FR1 and onwards:	x_mid = 3



The old result can be explained because AIMMS would use a reference to an unused memory location for bounds. Now AIMMS will use a reference to the parameters making up the range of the scalar variable. However, this implies a difference in the execution of AIMMS and may result in a difference in model results.



This option controls how you will be alerted against a potential difference in execution, depending on the following setttings:




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

*	With the option Maximal Number of Warnings Reported you can set the maximal number of warnings that are shown in errors/warnings and message window.




**Learn more about** 

*	:ref:`Options_Warnings_-_Maximal_Number_of_W`  
*	:ref:`Options_Warnings_-_Common_warning_default` 
*	:ref:`Options_Warnings_-_Strict_warning_default` 
*	:ref:`Options_Backward_Compatibility_-_Scalar_Suffix_Reference_Substitution` 
*	:ref:`Options_Warnings_-_Communicate_warnings_to_end_users` 



