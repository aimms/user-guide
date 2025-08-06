

.. _Composite-Table_Composite_Table_Properties_-_I:


Initial Sort
============

**Description** 

On the Initial Sort tab you can specify the sort criteria, that are used when the Composite Table is re-opened. This initial sort will be used until the user re-sorts the data by hand via a click in one of the column headers.

The initial sort criteria are defined by a user-specified sequence of columns. The rows in the table are then sorted based on the values in the first column in this sequence, if the values in the first column are equal, then the second column in the sequence is used, and so on. Per column the values are compared using a standard comparison function, which depends on the type of data displayed, but you can change the 'direction' of the sort (for example small-to-large vs. large-to-small).

If the contains the values of a numerical identifier, then the numbers in the column are compared. If the column contains strings, then these strings are sorted alphabetically. If the column contains element names, then these elements are sorted according to the set ordering.





