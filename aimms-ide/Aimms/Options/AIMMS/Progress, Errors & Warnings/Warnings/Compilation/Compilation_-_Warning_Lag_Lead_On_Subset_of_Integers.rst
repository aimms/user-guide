

.. _Options_Compilation_-_Warning_Lag_Lead_On_Subset_of_Integers:


Warning Lag Lead on subset of Integers
======================================



**Type**:	Selection	

**Range**:	The settings listed below	

**Default**:	Warning_in_develop_else_off	



In the AIMMS syntax the + is a **Lead**  operator when the left operand is an element valued expression, and similarly the - is a**Lag**  operator.

If the range of this element valued expression is a subset of Integers, in some situations the result may not be what you expect at first sight.

AIMMS now gives a warning when it encounters such a construct. It is not necessarily wrong, but the warning might help you to double-check whether the expression is doing what you expect.

With the option Warning_lag_lead_on_subset_of_integers, you can control whether you want to see this warning.





Let's inspect the following examples:



**Declarations:** 



	Set S {

	 subset of : Integers;

	 parameter: epS;

	 initial data: data { 10, 12, 14, 16 }

	}

	ElementParameter epS {

	 range: S;

	}

	Parameter X; 





**Example 1:** 

	epS := 12;

	X := epS + 2;



	This results in X = 16. First the Lead operation is performed and then a Val() function is applied to cast the element expression on the left to the numerical value on the right.

	Written out explicitly, the statement is thus the same as: X := Val( epS + 2 );





**Example 2:** 

	epS := 12;

	X := epS - 2;



	This results in X = 0. The statement is equivalent to X := Val( epS - 2 ). 

	(epS - 2) result in the empty element, because '12' is the second element in the set, and Val( 'empty element' ) is defined to be 0.







Please note that it is only since AIMMS version 4.39 that AIMMS does this correctly. In older versions of AIMMS the compiler sometimes(!) interpreted the + and - in these situations as a numeric + or -.

In the above two example, the equivalent statement for the old compiler are:

	

**Example 1:** 

	X := val(epS) + 2;

	

	This results in 14.



**Example 2:** 

	X := val(epS) - 2;



	This results in 10;





	

The differences between these two implementations of the compiler only give problems in two situations:

- if the subset of Integers on which the statement operates is a non-consecutive range, and/or 

- if the lag or lead operator results in the empty element because you exceed the first or last element of the set.





If in a certain expression you intended to use the numeric + or - (as the old compiler was doing), you can force that behavior by adding the Val( ) function yourself.







Possible values for the option:




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



