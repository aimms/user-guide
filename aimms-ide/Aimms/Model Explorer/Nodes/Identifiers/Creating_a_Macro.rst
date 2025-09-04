.. |img_def_Identifier_Macro_bmp| image:: images/Identifier_Macro.bmp


.. _Model-Explorer_Creating_a_Macro:


Creating a Macro
================

**Description** 

To create a new macro in the Model Tree:

1.	Select the position in a Declaration Section where the new macro should be inserted

2.	From the Edit menu select Insert – Other (or press the ``<Insert>``  key)

3.	In the dialog box select |img_def_Identifier_Macro_bmp| Macro and press OK

4.	Enter a name for the new macro

5.	Press ``<Enter>``  to create the new macro (or press ``<Esc>``  to abort the operation)



The newly created macro is not yet ready for use, because you should at least specify its definition attribute. To modify the attributes of the newly created macro:

*	Press ``<Enter>``  or double click on the macro node.




The most commonly used attributes of a macro are discussed below. 




*	``ARGUMENTS``: In the ``ARGUMENTS`` attribute, you can specify the argument names in terms of which the ``MACRO`` definition can be formulated.
*	``DEFINITION``: The ``DEFINITION`` attribute should contain the replacement text that is substituted when the macro is used in the model text. References to arguments in this definition are replaced with the calling arguments of the macro.




**How to ...** 

*	:ref:`Model-Explorer_Creating_New_Nodes`  




**Learn more about** 

*	:ref:`sec:expr.macro`  
*	:ref:`aimmshelp6-Model_Explorer_Attribute_Forms`  
*	:ref:`Model-Explorer_Attribute_Form_Manipulation`  



