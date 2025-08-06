

.. _Identifier-Selector_Making_Data_Changes_in_a_View_:


Make Data Changes in a View Window
==================================

**Description** 

Besides viewing the attribute values of the identifiers, you can also edit them directly in a View Window:

1.	Select the specific cell in the View Window

2.	From the Edit menu, select Rename/Edit (or click a second time in the cell)

If the cell is a valid identifier/attribute combination, a small edit window will appear.

3.	Modify the attribute value

4.	Press Enter (or click outside the cell)



All the modifications that you make to the attribute values in a View Window are maintained locally within the window and not yet passed on to the model. As in an attribute form of an identifier, you can use the four buttons in the upper-right of the window to:

*	Check all changes
*	Check all changes and close the window
*	Commit all changes without checking and close the window, or
*	Discard all changes




**Note** 

*	For some combinations of identifier and attribute AIMMS offers a wizard to help you filling in the attribute value. To use this wizard, you first select the specific cell and then select the Wizard command from the Edit menu.
*	If a column in a View Window represents an attribute that is not applicable for a specific identifier in a row, then the corresponding cell in the window is not editable.
*	If you try to remove a row or column in the View Window in which you have edited one of the cells, then AIMMS will ask you what to do with these changes.
*	For those identifiers that do not appear as nodes in the model tree (indices and element parameters that are declared on the attribute form of a set), it is not possible to make data changes in a View Window.




**Tips & Tricks** 

*	If you are editing a specific cell (the cell is in edit mode), then you can use the up and down arrow keys to directly switch to another cell. This other cell will then also be in edit mode
*	In a View Window you can easily copy attribute values from one cell to another. If you want to copy the entire contents of a cell, then you do not need to set either of the cells in edit mode, but you can directly drag the entire cell to another cell.
*	If one of the columns displays an attribute whose value may consist of more than one line of text (for example the Definition attribute), then the View Window will initially decide how many lines each row in the window should occupy. If you want to change the number of lines that are shown for a specific row, then you can use the '+' and '-' keys on the numerical part of the keyboard to increase or decrease this number of lines.
*	If you are editing a cell that may contain multiple lines of text, then the small edit window is slightly different from the edit window that is used for a single line attribute. The edit window has a small border, which can be used to (temporarily) resize the window to make editing more convenient. When you are finished editing and click outside the edit window, then the cell will return to its original size and position.



