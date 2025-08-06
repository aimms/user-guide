

.. _Table_Table_in_User_Mode:


User Mode
=========

**Description** 

In user mode you can make changes to individual cells in the table by simply selecting the cell and typing a new value for it. If you want to modify the current value without retyping it completely, you should select the cell and press the F2 key.

In addition to single cell edits, you can also select a whole block of cells. This selected block of cells can be used for:

*	cut, copy and paste operations,
*	entering one value for the entire block, or
*	deleting all values in the block (setting them to their default value)




**Note** 

*	If you do not want your users to be able to modify a whole block of cells at once, you can disable this feature using the option Allow Multiple Cell Changes in the properties dialog box.
*	You can only change the value of an identifier if the table is not read-only and if the identifier is in the set CurrentInputs, which generally means that the identifier should not have a definition.
*	When copying to another AIMMS table, realize that you should also specify the size you want to paste the information in. AIMMS does not automatically paste in the same size as Excel does.
*	It is also possible to copy data from a table (with or without header information) to an Excel spreadsheet.




**How to ...** 

*	:ref:`Model-Explorer_Cut_Copy_Paste_and_Delete`  
*	:ref:`Miscellaneous_Undo_Edit`  
*	:ref:`Table_Copying_data_from_an_AIMMS_tab`  




**Learn more about** 

*	:ref:`Table_Table_Introduction`  






