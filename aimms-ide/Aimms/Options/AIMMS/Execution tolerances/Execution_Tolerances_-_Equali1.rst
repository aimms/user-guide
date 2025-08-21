

.. _option-AIMMS-equality_relative_tolerance:


Equality Relative Tolerance
===========================



:Type:	Floating point number	
:Range:	[0.0, 0.9]	
:Default:	1e-13	



For two real numbers x and y the result of the comparison x < y (or any of the other relational operators =, <>, >, >=, or <=) depends on two tolerances:

*	Equality Absolute Tolerance, and
*	Equality Relative Tolerance.

For a detailed description of these two tolerances and numerical comparison in AIMMS, you should read the corresponding section in the Language Reference.





**Note** 

*	This option has no influence on the feasibility of constraints.
*	This option influences assignments in the following way; when a value is assigned to an identifier that is equal to the default of that identifier, equal within the above tolerances, the assignment will be ignored.




**Learn more about** 

*	:ref:`option-AIMMS-equality_absolute_tolerance` 
*	:ref:`comparing_numerical_values`  



