

.. _Options_Backward_Compatibility_-_Element_sequence_always_include_upper_bound:


Element sequence always include upper bound
===========================================



**Type**:	Selection	

**Range**:	One of the settings listed below	

**Default**:	Off	



An element sequence can be specified using the syntax { lo .. up by incr }.  Even when there was no integer i such that up = lo + incr * i, AIMMS used to include up in the generated sequence. For example, { 1 .. 8 by 2 } generates the elements { 1, 3, 5, 7 } when this option is off and { 1, 3, 5, 7, 8 } when this option is on. Now this depends on the setting of this option. Possible values are:



*	On  Include up even when up is not in the sequence defined by lo and incr.
*	Off  Include up only when there is an integer i such that up = lo + incr * i.




**Learn more about** 

*	:ref:`Options_Compilation_-_Warning_element_sequence_upperbound_not_included` 



