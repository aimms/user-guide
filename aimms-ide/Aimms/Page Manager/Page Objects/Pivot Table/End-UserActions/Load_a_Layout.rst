.. |img_def_Button_-_Load_State_jpg| image:: images/Button_-_Load_State.jpg


.. _Pivot-Table_Load_a_Layout:


Load a Layout
=============

The pivot table will only read in a state file (if present) during initialization (i.e. when the page is opened). When the end-user has altered the layout of the pivot table (e.g. by moving headers -using drag and drop - or by changing column widths) he may restore a previously saved layout by clicking the Load Layout button |img_def_Button_-_Load_State_jpg| in the upper left corner of the pivot table. This will show a drop-down menu containing one or more of the following commands (depending on whether or not a developer state and/or an end-user state has been saved for the selected pivot table).




*   **Load Default Layout**. This menu command is always present and will reload the pivot table as if no state file was present. The layout will be similar to that of newly created pivot tables. Amongst others, this means that both the row and column tree will contain at most one index and that all column widths are reset.




*   **Load Last Saved Developer Layout**. This menu command is only available if the application is running in end-user mode and a developer state (for the selected pivot table) is present. It will load the layout that had been saved by the developer.




*   **Load Last Saved User Layout**. This menu command is only available if an end-user state (for the selected pivot table) is present.



**Learn more about** 




*   :ref:`Pivot-Table_General2` 


*   :ref:`Pivot-Table_SaveaUser-SpecifiedLayout` 

