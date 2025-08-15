

.. _Options_Case_Management_-_Case_Ensure_Subset_Consistency_Method:


Case ensure subset consistency method
=====================================



**Type**:	Selection	

**Range**:	The settings listed below	

**Default**:	Remove elements from subsets



This option determines how subset consistency is attained at the end of loading a case.



Subset consistency ensures that for an element ``e``  in a set ``S`` , the element ``e``  is also present in the domain set ``D``  of ``S`` . Subset consistency is important for the correct behaviour of the AIMMS execution engine.



When an element ``e``  is present in a set ``S`` , but not in the domain set ``D`` , subset consistency can be attained by either inserting the element ``e``  into the domain set ``D``  or removing element ``e``  from set ``S`` . Inserting the element into the domain set corresponds with the option setting 'insert elements into domain sets'. Removing elements corresponds to the option setting 'Remove elements from subsets'. This last setting results in behaviour similar to the behavior of AIMMS 3.8, AIMMS 3.9 and AIMMS 3.10. When this option is set to 'ignore', subset consistency at the end of loading a case is not enforced. This 'ignore' setting results in behaviour similar to the behaviour of AIMMS 3.7 and earlier AIMMS releases.

 

*	Insert elements into domain sets
*	Remove elements from subsets
*	Ignore







**Note** 

*	See also option warning ensuring case consistency.






