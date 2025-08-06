.. |img_def_Button_-_Close_jpg| image:: images/Button_-_Close.jpg
.. |img_def_Button_-_Open_jpg| image:: images/Button_-_Open.jpg
.. |img_def_Button_-_Filter_jpg| image:: images/Button_-_Filter.jpg


.. _Pivot-Table_General2:


General
=======

On the General tab you can specify various color and font settings, as well as the degree in which an end-user can modify the pivot table and/or save the state of the pivot table.



**Background Color** 



The color that you specify here will be used to color the entire background of the Pivot Table. You see this color at the borders of the objects, in between the Outer Area and the Column Area etc. If not overruled, then it will also be used to color the background of the Row, Column, Outer and Grid areas.



If you do not specify this background color, the background is transparent: i.e. the color and drawing objects of the underlying page area will be visible.



**Border Color** 



This color will be used to color the line of the border around the Pivot Table. Please note, that this border color is only used when the border itself is specified to be a 'Line' border (on the :ref:`Pivot-Table_Object_Properties_-_Border`  tab). 



**Font** 



The font that you specify here will be used throughout all areas of the Pivot Table, unless you specify an alternative font for any of these areas.



**Multiple Case View** 



With this option you can set whether or not the Pivot Table should show the values for the cases in the current Multiple Case selection instead of only the values of the actual data in the model. Please note, that the end-user may overrule this setting using the Pivot Table Options dialog.



**Show Inactive Data** 



With this option you can control whether or not the Pivot Table should display inactive data. Identifier data will become inactive when elements are removed from the domain of the identifier. Note that, when this option has been set to "Yes", inactive set elements will only appear in the pivot table in case they have some inactive data associated with them.



**Dense Aggregation restricts to Domain** 



With this option you can control whether the domain condition as specified on the contents tab should be taken into account during dense computation of aggregated values. Note that in the pivot table, the domain condition is considered to be true for entries with a nondefault value. In case you want to achieve a situation in which the domain condition is considered to be true for entries with a nonzero value when using an identifier with a nonzero default (say condition(i,j)) you are advised to specify the domain condition in terms of a GUI expression of the form '1 onlyif ( condition(i,j) <> 0 )'.



For backward compatibility reasons this option will be set to "No" for pivot tables that have been created with AIMMS version 3.8.3.9404 (and earlier). For newly created pivot tables this option is initialized to "Yes".



**Only Rows with Differences** 



If you set this option to 1, the Pivot Table will not display any row for which all values in that row are equal. Note that if a row contains default values (which are perhaps not visible) as well as non-default values the values are not equal. This property is especially convenient to locate differences between cases in a multiple case view, where the cases are presented as columns.



Please note, that the end-user may overrule this setting using the Pivot Table Options dialog.



**Only Columns with Differences** 



Similar as for the rows, described above.



**Maximum Number of Tree Entries** 



This option allows the developer to specify the maximum number of displayed entries in the row and column tree (i.e. rows in the row tree and columns in the column tree). If the data that is contained in the pivot table is high-dimensional and the developer has not restricted the end-user access to the indices tab and/or the possibility to move indices around, the end-user could create a pivot table of unmanageable size (e.g. by making all indices dense and moving them to the same tree). The number of entries in the tree is estimated by multiplying the cardinality of all dense indices in the specific tree.When this maximum is exceeded the pivot table will not be displayed. Instead a message will be displayed stating that the number of rows (or the number of columns) exceeds the specified maximum. The default for the maximum number of tree entries has been set to 10000. This maximum number can be specified as a constant number or by a scalar numerical identifier. Note that the maximum number of tree entries is determined once, during initialization of the pivot table object, and will not be updated as the corresponding model identifier changes.



**User Modifications** 



If you (the developer) do not want your end users to be able to use all the end user features of the Pivot Table, you disable some of these features here:



**User Modifications - User Dialog** 



If you disallow the User Dialog, the dialog button will not be available. This implies that you also disallow the 'Creating Aggregators', 'Indices Showing All Elements', 'Switch to Multiple Case View' features, that are described below.



**User Modifications - Create Aggregators** 



In the Pivot Table Options dialog, the end user itself can specify aggregators for the indices in the table. If you disallow this, the dialog will not have the corresponding 'Tab'.



**User Modifications - Indices Showing All Elements** 



In the Pivot Table Options dialog, the end user itself can specify whether he wants to see all elements of a specific index (regardless of the sparsity). If you disallow this, the corresponding controls in the dialog will be disabled.



**User Modifications - Drag & Drop Headers** 



By default, the end user is allowed to drag and drop index headers from and to the Row, Column and Outer areas of the table, and thus rearrange the view. If you disallow dragging and dropping headers, the table always will have the view that you specified at design time.



**User Modifications - Open & Close Tree Nodes** 



By default, the end user is allowed to open and close nodes in the row and column tree, either by using the |img_def_Button_-_Close_jpg| or |img_def_Button_-_Open_jpg| buttons or by pressing the corresponding keyboard shortcut (``<Ctrl>``  - ``<arrow>`` )). If you disallow this, all open and close buttons will be removed from the pivot table and the keyboard shortcuts to open and close the tree will not be functional.



**User Modifications - Fixing Elements in Rows or Columns** 



If you disallowed this feature, the small 'filter buttons' |img_def_Button_-_Filter_jpg| to the left of the Row and above the Column area will not be displayed, and thus the end user cannot fix certain levels in the row or column trees to some specific elements only. See also: :ref:`Pivot-Table_ElementFixing` 



**User Modifications - Index Filtering** 



If you disallowed this feature, the end user will not be able to specify filters on the indices in the table. See also: :ref:`Pivot-Table_PivotTable_Index_Filtering`  



**User Modifications - Sorting Rows or Columns** 



By default, the end-user is allowed to resort rows and/or columns by drag-and-drop or by pressing the sort-button that is available in the cell in the row or column tree that has been selected. Use this option to control the ability of the end-user to change the display order of elements in the row and/or column tree.



**User Modifications - Insert Row or Column** 



By default, the end-user is not allowed to manually insert rows/columns in the current view of the data. See also: :ref:`Pivot-Table_PivotTable-InsertDelete` 



**User Modifications - Delete Row or Column** 



By default, the end-user is not allowed to manually delete rows/columns in the current view of the data. See also: :ref:`Pivot-Table_PivotTable-InsertDelete` 



**User Modifications - Switch to Multiple Case View** 



In the Pivot Table Options dialog, the end user himself can specify whether he wants the table to display multiple cases. If you disallow this, the corresponding controls in the dialog will be disabled, and whether or not the table is in Multiple Case View is solely determined by the property Multiple Case View described above.



**Save Layout/State** 



The pivot table is customizable by the end user in various ways. Because you do not want to make the same customizations over and over again each time that you have closed and re-opened a page, the pivot table allows you to save the current Layout or State. This state info is saved into a file that is separate from the project file itself, and Aimms distinguishes between a developer state file and an end-user state file.



The following information is saved in the state file:


*   The locations of the indices in the various areas of the Pivot Table (the result of the dragging operations)
*   All options specified through the Option Dialog (aggregators, multiple case view, dense indices, only differences, etc)
*   You can also choose to save the current layout of both the row and column tree (which branches are collapsed, which nodes are fixed, and the individual width of column entries). Please note that this info can be rather large in size.
*   The last sort that has been applied. In case the current layout has not been stored in the state file, the last sort is re-applied when the data that is displayed in the pivot table changes.



The properties below are available to control the saving of the Layout or State. Furthermore, in the Tools menu, the :ref:`Miscellaneous_State_File_Manager`  is available. Saving/loading and deleting states can also be managed by the Search for Pivot Table State functions that can be found in the AIMMS Function Reference.



**Save Layout/State - By End User** 



This property defines whether or not an end-user of your Aimms application is allowed to save the modification that he makes in the pivot table. It can be set to the following values:


*   No: no end user state will not be created	


*   On Demand: the end user should save a specific state explicitly. This can be done via a procedure created by the developer, containing the PivotTableSaveState function, or via the menu command View – Save User State. Please note that if you have a user specified menubar on your page you need to include this command in that menubar.


*   When page is closing: the current state is saved automatically when the page containing the pivot table is closed (this is the default setting)



**Save Layout/State - Store Entire Tree Layout** 



When selected, this property will make sure that the current layout of both row and column trees is saved as well. The entire tree layout includes column widths, the ordering of nodes in the row and column trees as well as whether nodes are opened or closed.



**Save Layout/State - By Developer** 



This property defines whether the developer can save the modifications that he makes in the Pivot Table when the page is in user mode. This state will be used each time the developer re-opens the pivot table, but it will also be used as the initial layout for the very first time that an End User opens the pivot table. Of course, as soon as the End User saves his own state later on, the developer state will be ignored.

This property can have the following values:


*   No: no developer state will be created. During development the pivot table will handle the state as if the project is in End User mode, and thus use the setting of the property "By End User"
*   On Demand: the developer should save a specific state explicitly. This can be done via a procedure created by the developer, containing the PivotTableSaveState function, or via the menu command View – Save Developer State.
*   When being saved: the state is saved at the same time as when the page containing the pivot table is saved. When this setting is used, any modification to the Pivot Table state will set the "is changed" flag of the containing page.



**Save Layout/State - Specific State Name** 



By default Aimms will generate a unique name for each pivot table and use that name to save and retrieve the state of the table in the end-user or developer state file. If you want to have two pivot tables on separate pages to use the same state, you may enter a name yourself and use this name in both pivot tables. This is especially convenient for a pivot table on a print page: A pivot table on a print page cannot be modified directly because all objects on a print page are 'display-only', but you can prepare a specific layout to be printed on a regular page and use the saved state from that page to open the print page in that same layout.



