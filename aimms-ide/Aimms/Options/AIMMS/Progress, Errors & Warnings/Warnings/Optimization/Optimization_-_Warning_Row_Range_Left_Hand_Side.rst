

.. _Options_Optimization_-_Warning_Row_Range_Left_Hand_Side:


Warning Row Range Left Hand Side
================================



Type:	Selection	

Range:	The settings listed below	

Default:	Strict_warning_default	



At the end of the first generation of a mathematical program, individual constraints are checked whether or not they are binding by computing the range of the left hand side and comparing it to the right hand side. Consider the following example, where b1 and b2 are binary variables:



  CONSTRAINT:

  	identifier : eqn

  	definition : b1 + b2 <= 3



AIMMS will issue the warning message: The range of the left hand side of the "<=" constraint eqn is [0, 2], and the right hand side of that constraint is 3; this constraint is non-binding.



The option "``Warning_Row_Range_Left_Hand_Side`` " determines how non-binding constraints are reported, depending on the following settings:




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

*	The option Warning Row Range Left Hand Side is the complement of the option Row Range Violation Left Hand Side.
*	With the option Maximal Number of Warnings Reported you can set the maximal number of warnings that are shown in errors/warnings and message window.




**Learn more about** 

*	:ref:`Options_Warnings_-_Maximal_Number_of_W` 
*	:ref:`Options_Warnings_-_Common_warning_default` 
*	:ref:`Options_Warnings_-_Strict_warning_default` 
*	:ref:`Options_Warnings_-_Communicate_warnings_to_end_users` 
*	:ref:`Options_Optimization_-_Row_Range_Violation_Left_Hand_Side` 






