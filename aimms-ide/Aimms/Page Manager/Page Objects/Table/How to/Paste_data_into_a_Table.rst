

.. _Table_Paste_data_into_a_Table:


Paste data into a Table
=======================

When pasting a block of data into a table, the following applies



1.	If the source block area consists of a single cell, the copied data is pasted into every (updatable) cell in the destination area.

2.	If the destination block area consists of a single cell, the area is extended to fit the copied contents (within the boundaries of the table itself).

3.	If the destination block area is (in at least one dimension) larger than the source area, the excess part of the destination block will not change (unless the source area consist of a single cell (see point 1))

4.	If the destination block area is (in at least one dimension) smaller than the source area, no data will be pasted outside the destination area and not all copied data will be pasted (unless the destination area consist of a single cell (see point 2))



Of course, cells that contain data that is not updatable will be skipped during pasting. After pasting, the selection will consist of the pasted area.





