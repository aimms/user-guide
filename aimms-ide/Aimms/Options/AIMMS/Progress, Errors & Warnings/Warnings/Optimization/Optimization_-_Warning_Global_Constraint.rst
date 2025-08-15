

.. _Options_Optimization_-_Warning_Global_Constraint:


Warning Global Constraint
=========================



**Type**:	Selection	

**Range**:	The settings listed below	

**Default**:	Common_warning_default



For each global constraint it is verified whether or not it is binding. Consider the following examples:



CONSTRAINT:

  identifier : ad

  definition : cp::AllDifferent(i,v(i))



When the set that is the scope of index i is empty, AIMMS will issue the following warning "The cp::AllDifferent constraint does not need to restrict the value of any variable which makes it nonbinding.".



In the following constraint, the number of occurrences in a subsequence is always between 0 and the sequence length.



CONSTRAINT:

  identifier : seq

  definition : cp::Sequence(

             inspectedBinding : k,

             inspectedValues : v3(k),

             lookupValues   : lv,

             sequenceLength  : 3,

             lowerBound    : 0,

             upperBound    : 3,

             cyclic      : 0)



For the above constraint AIMMS will issue the warning: "cp::Sequence(): With a zero lowerbound and a sequence length 3 and upper bound 3 this constraint becomes nonbinding."



The option "``Warning_Global_Constraint`` " determines how nonbinding global constraints are reported, depending on the following settings:




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
*	:ref:`Options_Optimization_-_Warning_Row_Range_Left_Hand_Side` 
