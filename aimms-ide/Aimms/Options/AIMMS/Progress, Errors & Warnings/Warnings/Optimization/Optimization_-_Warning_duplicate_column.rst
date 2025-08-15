

.. _Options_Optimization_-_Warning_duplicate_column:


Warning Duplicate Column
========================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Common_warning_default



At the end of generating a linear mathematical program, AIMMS checks whether it contains duplicate columns. Two columns are duplicates when they contain the same coefficients in the matrix for each row.



The consequences of duplicate columns are:

*	An increase in the size of the mathematical program, and therefore an increase in memory consumption.
*	More important is that duplicate columns can lead to non-unique solutions, and consequently small changes in data or a change of solver may lead to a different solution.




Potential causes of duplicate columns are:

*	An incomplete index domain condition on one of the variables.
*	The data used to create this instance contains duplicate information for selected elements. 
*	A modeling error; one of the columns should also be present in another constraint.




The option ``Warning_duplicate_column``  determines how duplicate columns should be reported, depending on the following settings:






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
*	:ref:`Options_Warnings_-_Communicate_warnings_to_end_users` 



