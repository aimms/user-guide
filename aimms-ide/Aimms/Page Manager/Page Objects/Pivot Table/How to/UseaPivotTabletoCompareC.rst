

.. _Pivot-Table_UseaPivotTabletoCompareC:


Use a Pivot Table to Compare Cases
==================================

By carefully combining the multiple case view and aggregators, you can use the Pivot Table to visually compare the data in two or more cases. You can accomplish this as follows:




*   Add the explicit identifiers, or a subset of identifiers, that you want to compare to the Pivot Table




*   Set the Pivot Table in Multiple Case View. You can enter this setting design time in the :ref:`Pivot-Table_General2`  tab of the Properties dialog box, or an end-user can select setting in the :ref:`Pivot-Table_End-UserDialog` . This will add an additional case dimension to the Pivot Table.




*   Add the cases you want to compare to the multiple case selection using the menu item Data - Multiple cases. When the current case selection is empty, the pivot table will display the data of the active case only (as if the multiple case view was disabled).




*   If you only want to show the differences, you can select to only show the rows or columns with differences on the **General**  tab in the :ref:`Pivot-Table_End-UserDialog` , depending on whether the case index is part of the row or column index tree




*   If you want to display all the data in the cases, you can add a Difference aggregator to the case index if you are comparing just two cases, or a Range aggregator if you comparing more than two cases. You can add aggregators on the **Aggregators**  tab of the :ref:`Pivot-Table_End-UserDialog` .







