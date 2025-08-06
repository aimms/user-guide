

.. _Miscellaneous_Name_Completion:


Name Completion
===============

**Description** 

In attribute fields and in many of the dialog boxes of AIMMS, you often need to type the name of an existing identifier in your model. To help you in typing (long) identifier names and to prevent you from making typing errors, AIMMS has a Name Completion command.

When you press ``<Ctrl>+<Spacebar>``  anywhere in an edit field, AIMMS will try to complete any identifier name at the current cursor position, using only the first characters typed. If the typed characters cannot be completed uniquely, then a popup menu appears, showing a list of possible identifier names.

If you press ``<Ctrl>+<Shift>+``  ``<Spacebar>`` , then AIMMS will also complete keywords and predefined identifier, procedure and function names.

If the name at the cursor position already represents the complete name of an (indexed) identifier, then the popup menu with possible name completions also contains a command to extend the name with its index domain as specified in its declaration.



