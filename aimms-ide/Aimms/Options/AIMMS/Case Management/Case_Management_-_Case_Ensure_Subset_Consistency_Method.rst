

.. _option-AIMMS-case_ensure_subset_consistency_method:


Case Ensure Subset Consistency Method
=====================================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Remove elements from subsets



This option determines how subset consistency is attained at the end of loading a case.

Subset consistency ensures that for an element ``e`` in a set ``S``, the element ``e`` is also present in the
domain set ``D`` of ``S``. Subset consistency is important for the correct behaviour of the AIMMS execution engine.

When an element ``e`` is present in a set ``S``, but not in the domain set ``D``, subset consistency can be
attained by either inserting the element ``e`` into the domain set ``D`` or removing element ``e`` from set ``S``.
Inserting the element into the domain set corresponds with the option setting 'Insert elements into domain sets'.
Removing elements corresponds to the option setting 'Remove elements from subsets'.

Possible values are:

    *	Insert elements into domain sets
    *	Remove elements from subsets
    *	Ignore


**Note** 

*	See also the option **Warning Ensuring Case Consistency**.


**Learn more about** 

*	:ref:`option-AIMMS-warning_ensuring_case_consistency` 

