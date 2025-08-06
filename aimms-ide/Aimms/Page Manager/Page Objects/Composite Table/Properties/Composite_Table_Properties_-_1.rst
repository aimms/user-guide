

.. _Composite-Table_Composite_Table_Properties_-_1:


Contents
========

**Description** 

In the Contents tab of the Composite Table you can modify the identifier that is used for the domain, and you can add, modify or remove identifiers that are displayed as the columns of the Composite Table.



The domain identifier specifies which rows are shown in the Composite Table. There are two types of identifiers that you can use for the domain identifier:

*	An Index identifier, the rows in the table will then correspond to the element of the index set. These elements are displayed in one single domain column.
*	Any indexed identifier, the rows in the table will then correspond to the non-default tuples of this identifier. For every free index in the identifier a domain column is displayed. If you use an indexed identifier for the domain, the same indexed identifier will also be filled in as the first data column.




The column identifiers should have an index domain that matches the domain identifier. This means that the dimension of the column identifier cannot exceed the dimension of the domain identifier, and any free index in the column identifier should uniquely match with an index from the domain identifier. Thus, you can select a column identifier with a dimension that is less than the dimension of the domain identifier. In that case some values in the column may appear multiple times (as an extreme example: if you select a scalar identifier, then its value will appear on every row).





**Note** 

*	You can also add identifiers to a composite table by switching the page to edit mode and selecting and dragging multiple identifiers from the model tree into the composite table.






