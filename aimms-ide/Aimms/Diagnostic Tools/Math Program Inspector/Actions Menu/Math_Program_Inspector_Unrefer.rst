

.. _Diagnostic-Tools_Math_Program_Inspector_Unrefer:


Unreferenced Identifiers
========================

**Description** 

One of the causes of a faulty model may be that you forgot to include one or more variables or constraints in the specification of your mathematical program. The math program inspector helps you in identifying some typical omissions. By choosing the Unreferenced Identifiers command from the Actions menu, AIMMS helps you to identify

*	constraints that are not included in the constraint set of your math program while they contain a reference to one of the variables in the variable set,
*	variables that are not included in the variable set of your math program while a reference to these variables does exist in some of the constraints, and
*	defined variables that are not included in the constraint set of your math program.

The results of this action are visible through the Math Program Solution tab.





**Learn more about** 

*	:ref:`Diagnostic-Tools_Math_Program_Inspector_Math_Pr`  






