

.. _Composite-Table_Composite_Table_Properties_-_T:


Table
=====

**Description** 

The Table property tab contains Composite Table specific properties. You can adjust the following properties here:



**Header Bar** 

This option defines whether or not the Composite Table should display a header bar at the top. Since the end-user needs the header bar to sort the data and to rearrange the columns, turning this option off automatically disables these features.



**Horizontal Lines** 

When you choose this option, horizontal lines will separate the rows in a Composite Table.



**Vertical Lines** 

With this option you specify whether vertical lines should separate the columns in a Composite Table.



**Mark Entire Row** 

The current cell in the Composite Table is always marked by a small box. With this option, you can choose to let the Composite Table also mark the entire row in which the cell is contained. This is especially useful if the table is rather wide.



**Header Re-arrange** 

With this option switched on, the end-user is able to rearrange the columns in a Composite Table by dragging the name in the header bar to the desired position.  Note that this option is ignored if you choose not to display the Header Bar.



**Add/Remove Columns** 

This option enables the :ref:`Composite-Table_Hiding_and_rearranging_columns_CompositeTable` dialog box. This dialog box pops up when the end-user right-clicks the mouse in the header bar of the composite table. The composite table does not remember the state of which columns were hidden when a page is closed and re-opened. However, this data can be stored by attaching identifiers to the :ref:`Composite-Table_Composite_Table_Properties_-_C`  status of the columns. 



**Column Sort** 

When you choose this option you will allow the end-user to Sort the Data. The end-user can sort the data by clicking on the column names in the header bar. Note that this option is ignored if you choose not to display the Header Bar.



**Cell Selection** 

This option determines whether the end-user is allowed to select individual cells (for editing). If this option is not selected, then the end-user can only select entire rows and it is not possible to edit any of the values in the columns. With this option you disallow cell selection for every column, if you only want to disallow the selection (and editing) of cells in specific columns, you should use the option Allow Cell Selection in the Columns tab.



**Row Selection** 

This option determines whether the end-user is allowed to select an entire row. If not selected, then the user can only select individual cells (unless this is disallowed also via the option Cell Selection, in which case the user can only view and scroll the table). If you want the end-user to be able to modify the domain of the Composite Table (adding, removing and modifying the rows), then the option Row Selection must be selected.



**Multiple Row Selection** 

If you allow the selection of multiple rows, then the end-user can use the Control and Shift keys in combination with mouse clicks to select more than one row in the Composite Table (which may be useful for deleting multiple rows at once). This option is ignored if the option Row Selection is not selected.



**Automatic Re-Sort** 

When you choose this option the data in the Composite Table will be automatically re-sorted when new data is available. The rows will be re-sorted using the last sort condition, which is either the Initial Sort or the last sort that the user has made (by clicking the column headers). Note that this option makes it difficult for the end-user to enter new values for all values in a column from top to bottom, because after each individual change the rows may be re-sorted and the last edited cell may thus 'jump' to another position.



**Show Inactive Data** 

If this option is not selected, inactive data will be considered to have a default value. In a Composite Table this means that inactive data in the domain identifier will not result in a row in the table, and inactive data in any of the column identifiers will be displayed using their default value. You can read more about inactive data in the Language Reference.



**Headers in Background Color** 

This option can only be set on a print page and it specifies that the headers should be printed in the background color, instead of grey. This can be useful when printed reports with composite tables need to be faxed.



**Note** 

*	When both the Cell Selection option and the Row Selection option are turned on, you can click to the left of the first element in a row when you want to select a row instead of the element in a row. When one or both of the options Cell Selection and Row Selection is turned off, you will notice that the small column at the left side of the Composite Table will disappear. 
*	When both the Cell Selection option and the Row Selection option are turned off, then the user cannot make any selection in the Composite Table.




**Learn more about** 

*	:ref:`Composite-Table_Sorting_Data_in_a_Composite_Ta`  
*	:ref:`Composite-Table_Adding_Modifying_and_Removing_`  
*	:ref:`Composite-Table_Composite_Table_Properties_-_I`  
*	:ref:`inactive_data`



