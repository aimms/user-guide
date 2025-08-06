

.. _Composite-Table_Adding_Modifying_and_Removing_:


Add Rows in a Composite Table
=============================

**Description** 

For a Composite Table it is possible to allow the end-user to add, modify or remove rows. Whether any of these actions is allowed is specified in the Domain tab of the Composite Table properties.

If you want to add a row to the Composite Table, you can click on a row that most closely matches the new entry and then press the Insert key. A small dialog box will appear in which you can specify the new element (or tuple).

If you want to remove one or more rows in the Composite Table, you can select the rows and press the Delete key.

If you want to modify a row in the Composite Table, you can click on the specific row and press the F2 function key. A small dialog box appear in which you can specify the modified element (or tuple).



If the domain identifier is an index, the changes in the rows will directly have effect on the set, this means, elements will be added, renamed or removed. If the domain identifier is an indexed identifier then the changes will have effect on the values of that identifier (it is not possible to introduce tuples with elements that were not already in the domain sets). This means that the identifier will get a default value for removed rows and a non-default value for added rows. For a numerical identifier, this non-default value is 1 (or 2, if 1 happens to be the default value). For a string valued identifier this non-default value is '*' (or '**', if '*' happens to be the default value). For an element parameter the default value is the first element in the corresponding set (or the second, if the first element is the default value), note that if this set is empty (or only contains the default element) then an Add or Modify of the domain does not work.



**Learn more about** 

*	:ref:`Composite-Table_Composite_Table_Properties_-_D`  
*	:ref:`Composite-Table_Composite_Table_Properties_-_T`  






