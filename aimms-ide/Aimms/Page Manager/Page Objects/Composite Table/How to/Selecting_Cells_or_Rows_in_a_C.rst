

.. _Composite-Table_Selecting_Cells_or_Rows_in_a_C:


Select Cells or Rows in a Composite Table
=========================================

**Description** 

Depending on the properties of a Composite Table, the user can either select individual cells or select one (or more) entire rows. Because some actions are only defined for selected rows (modifying the domain) and other only on the selected cell (modifying a value) you should understand how to make the proper selection.

If only the option Row Selection is specified (and not Cell Selection), then selecting a row is very intuitively: you simply click anywhere within the row, or use the up and down keys on the keyboard.

If only the option Cell Selection is specified (and not Row Selection), then selecting a cell is also very intuitively: you simply click on the specific cell, or use the arrow keys on the keyboard.

Only if both the options Cell Selection and Row Selection are specified, then selecting either a single cell or a row is a bit more difficult. In this case the Composite Table is automatically extended with a small extra column at the left side, so each row gets one extra artificial cell. If you try to select this artificial cell (either via a mouse click, or via the arrow keys on the keyboard) you automatically select the row instead.



