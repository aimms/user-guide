

.. _Options_Optimization_-_Warning_duplicate_row:


Warning Duplicate Row
=====================



**Type**:	Selection	

**Range**:	The settings listed below	

**Default**:	Common_warning_default



At the end of generating a mathematical program, AIMMS checks whether it contains duplicate rows.



The consequences of duplicate rows are:

*	An increase in the size of the mathematical program, and therefore an increase in memory consumption.
*	Solution time may increase, in particular when a non-linear program has been generated.
*	Duplicate rows lead to non-unique shadow prices.




Potential causes of duplicate rows are:

*	The data used to create this instance contains duplicate information for selected elements. 
*	There is an index in the index domain of the constraint which isn't used in the definition of that constraint.
*	There is a duplicate constraint formulation.




The option "``Warning_duplicate_row`` " determines how duplicate rows should be reported, depending on the following settings:






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



