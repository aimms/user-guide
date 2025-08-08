

.. _Identifier-Selector_Identifier_Selector:


Identifier Selector
====================

**Description** 

When you are developing or managing a large and complicated model, then you sometimes may need an overview of all identifiers that have some sort of similarity. For example, it may be important to simultaneous view

*	all the constraints in a model,
*	all variables with a definition,
*	all parameters using a certain domain index, or
*	all identifiers that cover a specific part of your model.




The Identifier Selector in AIMMS helps you to make these selections. The Identifier Selector window consists of a tree of Selector nodes, each of which (when applied) results in a specific list of identifiers in your model. There are eight types of selectors:

*	a node selector, where the list of identifiers is created via direct (static) references to nodes in the model tree,
*	a conditional selector, where the list of identifiers is created dynamically on identifier type and/or the contents of one of their respective attributes,
*	a set-dependency selector, where the list of identifiers is created dynamically on the basis of dependency of a specific set in either the identifier domain, identifier range, or a sub-/superset relation,
*	an element-dependency selector, where the list of identifiers is created by selecting all individual variables or constraints for which one of the indices has been fixed to a certain element,
*	a scale selector, where the list of identifiers is created dynamically on the basis of individual rows or columns in the generated matrix that may be badly scaled,
*	a status selector, where the list of identifiers is created dynamically on the basis of the status of a variable or constraint (either basic, feasible or at bound),
*	a value selector, where the list of identifiers consists of variables or constraints for which the value (or marginal value) satisfies some simple numerical condition, or
*	a type selector, where the list of identifiers is created dynamically on the basis of the type of a variable (e.g. continuous, binary, nonnegative) or constraint (e.g. less-than-or-equal, equal, greater-than-or-equal).




The tree structure of the Identifier Selector is not only used as storage for all created selectors, but its hierarchical structure can also be used to combine a number of selectors. The resulting list of identifiers is then constructed using standard set operations like add, subtract and intersect.





You can create duplicates of a selector node, so that the same node appears at multiple locations in the tree.





**Learn more about** 

*	:ref:`Identifier-Selector_Node_Selector`  
*	:ref:`Identifier-Selector_Conditional_Selector`  
*	:ref:`Identifier-Selector_Set_Dependency_Selector`  
*	:ref:`Identifier-Selector_Combining_Selectors`  
*	:ref:`Identifier-Selector_Using_Identifier_Selections`  
*	:ref:`Identifier-Selector_Identifier_Selector_-_Menubar`  
*	:ref:`Identifier-Selector_Identifier_Selector_-_Toolbar`  



