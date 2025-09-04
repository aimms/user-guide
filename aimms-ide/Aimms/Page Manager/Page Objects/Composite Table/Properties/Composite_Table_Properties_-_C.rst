

.. _Composite-Table_Composite_Table_Properties_-_C:


Columns
=======

**Description** 

In the Columns tab of the Composite Table properties dialog box, you can set options for each individual column. To do so, you first select the specific column in the drop-down list, and then adjust any of the following properties:



**Automatic Adjust upon Data Change** 

When you choose this option, the width of a column is adjusted automatically each time that new data for that column is available.



**As Percentage of Total Width** 

When you choose this option, the width specified in the initial field is a percentage of the total width of the composite table instead of a fixed width. It is possible to use fixed width for some columns and a percentage width for others. This option is particular useful in combination with resizable pages, because the width of the column will grow or shrink according to the new width of the composite table.



**Initial** 

In this field you can specify the initial width of the column associated with this identifier. This field may contain a number or a numerical identifier. When you specify the initial width using an identifier, this identifier will not only be used to derive the initial column width, but a change in column width will also be stored in that identifier. In this way you can store the last used column width, so that when the page is re-opened, its layout is the same.





**Hide** 

In this field you can specify whether this column should be hidden from the end-user. You can do this by entering a number or a numerical identifier. The value 0 means that the column is visible, other values mean that the column is hidden. This can be useful for example when you do not want the domain identifier to be visible or if you want to hide a column for a specific type of end-user. If you allow the end-user to hide columns through :ref:`Composite-Table_Hiding_and_rearranging_columns_CompositeTable` dialog box, then the choices in this dialog box are stored in the value of this Hide parameter. However, if the Hide property is specified by a literal number or by a non-updatable identifier, then the column hidden state cannot be altered by the end-user.

If you don't specify this Hide property, then the property inherits from the Hide property in the :ref:`Composite-Table_Composite_Table_Properties_-_C`  section



**Allow Cell Selection in this Column** 

This checkbox specifies whether the end-user is able to select (and edit) a single cell in the specific column. Note that this option is ignored if the general option Cell Selection is disabled (on the Table tab).



**Multiple Lines** 

This checkbox specifies whether a string should be shown completely using multiple lines. If this property is set, strings will be shown in multiple lines, based on end-of-line characters.





**Column Defaults - Hide** 

This field allows you to specify one identifier that handles the hidden status of all columns in the Composite Table. You can specify a one-dimensional identifier, indexed over a (subset of) AllIdentifiers. 

For example: 

If the composite table has columns: index ``i``, and parameter ``x(i)``, and 

the identifier for this property is ``myHiddenIdentifiers(IndexIdentifiers)``, 

then the hidden status of the column containing i is determined by the value of ``myHiddenIdentifiers('i')``.

Please note that:


*    you cannot use this to hide columns that represent an expression, instead of a direct identifier reference, and 
*    you cannot distinguish between several slices of the same identifier (for example: ``x('a')`` and ``x('b')``)



**Learn more about** 

*	:ref:`Composite-Table_Composite_Table_Properties_-_T`  
*	:ref:`Security_User_Management`  



