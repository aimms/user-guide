

.. _option-AIMMS-equality_absolute_tolerance:


Equality Absolute Tolerance
===========================



:Type:	Floating point number	
:Range:	[0, 1]	
:Default:	0	



For two real numbers x and y the result of the comparison x < y (or any of the other relational operators =, <>, >, >=, or <=) depends on two tolerances:

    *	Equality Absolute Tolerance, and
    *	Equality Relative Tolerance.

For a detailed description of these two tolerances and numerical comparison in AIMMS, you should read the corresponding :ref:`section <comparing_numerical_values>`
in the Language Reference.


**Note** 

*	This option has no influence on the feasibility of constraints.
*	This option influences assignments in the following way; when a value is assigned to an identifier that is equal to the default of that identifier, equal within the above tolerances, the assignment will be ignored.
*   This option also affects WinUI objects that display a numerical value as a check box (such as check box columns in a table). The check box is shown as unchecked only if the value is equal to zero within this tolerance. A value that is close to zero but exceeds this tolerance is therefore treated as nonzero and shown as checked.
*   The :any:`DISPLAY` statement shows values within this tolerance as 0. Values outside this tolerance are shown as they are stored.


**Learn more about** 

*	:ref:`option-AIMMS-equality_relative_tolerance` 
*	:ref:`comparing_numerical_values`  
