

.. _Diagnostic-Tools_Math_Program_Inspector_Substru:


Substructure Causing Unboundedness
==================================

**Description** 

When the underlying math program is unbounded, the math program inspector follows a straightforward procedure. First, all infinite variable bounds are replaced by a big constant M. Then, the resulting model is solved, and all variables that are equal to this big M are bookmarked in the tree as being the Substructure Causing Unboundedness. In addition, all constraints that contain at least two bookmarked variables are bookmarked too.



**Learn more about** 

*	:ref:`Diagnostic-Tools_Math_Program_Inspector_Bookmar` 
*	:ref:`Diagnostic-Tools_Math_Program_Inspector_Tree_Vi`  






