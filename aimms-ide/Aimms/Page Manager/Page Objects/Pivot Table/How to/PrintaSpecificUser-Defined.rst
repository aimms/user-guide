

.. _Pivot-Table_PrintaSpecificUser-Defined:


Print a Specific User-Defined Layout
====================================

When a Pivot Table is contained on a print page, AIMMS does not directly allow you to change the layout of that Pivot Table, as you can on an ordinary end-user page. By following the procedure outlined below you can still print a Pivot Table according to the given end-user determined layout.




*   Create an end-user page containing a Pivot Table object




*   Associate a state file with the Pivot Table, and allow the end-user to save the state of the Pivot Table




*   Recreate the Pivot Table object on a print page (e.g. by copying the table from the end-user page, and copying it onto the print page)




*   By saving the state on the end-user page, AIMMS will automatically use this state when printing the print page to print the Pivot Table according to the layout stored in the state file



**Learn more about** 




*   :ref:`Template-Manager_Print_Templates_Introduction` 
*   :ref:`Pivot-Table_SaveaUser-SpecifiedLayout` 

