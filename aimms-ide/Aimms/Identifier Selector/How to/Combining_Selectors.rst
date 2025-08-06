

.. _Identifier-Selector_Combining_Selectors:


Combine Selectors
=================

**Description** 

The tree structure in the Identifier Selector implicitly creates combinations of selectors by applying one of the set operations union, difference or intersection. The root of the tree consists of the (fixed) selection of all model identifiers. For each subsequent child node you have to indicate how this selector node should modify the list of identifiers that is defined by the parent node. You can choose to

*	Add the identifiers defined by the child selector node, or
*	Subtract the identifiers defined by the child selector node, or
*	Intersect with the identifiers defined by the child selector node.

The type of the set operation applied is indicated in the icon of each node in the selection manager. An Add operation is indicated by a small + (plus) sign, a Subtract operation by a small – (minus) sign, and an Intersect operation by a small x (multiplication) sign.





**How to …** 

*	:ref:`Identifier-Selector_Changing_the_type_of_set_opera` 



