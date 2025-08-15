

.. _Pivot-Table_Contents:


Contents
========

On the contents tab, you specify which identifiers are displayed in the Pivot Table. Furthermore you can specify various identifier dependent properties.



**Implicit Identifiers** 



Here you can specify a subset of AllIdentifiers. If specified, the Pivot Table will be filled with all identifiers that are contained in this subset. If you use this in combination with a Selection object in which the end user can alter the contents of this subset, then you can create a very flexible view in which the user itself can determine which identifiers he wants to see. Please note, that if you specify this property, this affects how the list of Explicit Identifiers will be interpreted (see below).



**Explicit Identifiers** 



This property is treated slightly different depending on whether or not you have specified the property Implicit via Subset above.



If you do not specify Implicit via Subset then the Pivot Table will contain only those identifiers that you specify here explicitly. 

Otherwise, the identifiers that you specify here are only used for applying properties for identifiers that are already part of the given subset of AllIdentifiers. If you specify an identifier that is not in this subset, it will not be added to the pivot table and its properties will be ignored (until the identifier is added to the subset later).



You can enter any data identifier from your model, optionally with some of its indices fixed. If you fix the elements of an identifier that is contained in the subset specified for the Implicit Identifiers property, then the sliced identifier will be added to the Pivot Table instead of the entire full-domain identifier.



In the sub tree below each Explicit Identifier you can specify various identifier related properties.



**Explicit Identifiers - Unit** 



This property is only available if the specified Explicit Identifier has a unit in your model. The property allows you to display the values of the identifier in terms of another commensurate unit.



**Explicit Identifier - Show Unit** 



This property is only available if the specified Explicit Identifier has a unit in your model. The property allows to control where the unit information will be shows. You can decide to



1.	hide the unit information,

2.	show the unit information in the header corresponding to the Identifier index, or

3.	show the unit in every individual grid cell.

	

If not specified the corresponding property in the Defaults section is used.



**Explicit Identifier - Show Unit - Use Brackets** 



This property is only available if unit information is shown for the specified Explicit Identifier (either in the header or in every individual grid cell). The property allows you to display the unit without or in between square brackets. If not specified the corresponding property in the Defaults section is used.



**Explicit Identifier - Show Unit - Text Override** 



This property is only available if unit information is shown for the specified Explicit Identifier (either in the header or in every individual grid cell). The property allows you to override the unit string that is being displayed via a static string or a quoted text.



**Explicit Identifiers - Title** 



With this property you can specify an alternative name for the identifier in the Pivot Table.



**Explicit Identifier - Domain** 



With this property you can control what values of the Explicit Identifier are displayed in the pivot table. The domain of the identifier should match the domain of the Explicit Identifier itself (apart from some permutation). If not specified the pivot table will by default only display rows and columns that contain at least one nondefault value. If specified, the pivot table will show all entries for which the Domain contains a nondefault value. Note that this means that the pivot table will also display rows and columns for which the Explicit Identifier doesn't contain any nondefault value in case the Domain does contain some nondefault value. Note also, that when the end-user decides to display the indices as dense, this will result in all rows and columns being displayed, including the ones for which the Domain only contains default values.



**Explicit Identifier - Store Selection in** 



With this property you can specify an identifier with the same index domain as the explicit identifier itself (or a permutation thereof) that will be linked to the selection in the pivot table. For every selected grid cell, the corresponding entry in the selection identifier will have a value of 1 (and 0 otherwise).



For example, you can use this identifier to see what cells have been selected when the **Procedure**  - **On Select**  is called.



**Explicit Identifiers - Format** 



The properties in the Format category define how the values of the identifiers are displayed. If not specified, then the specific format property is inherited from the corresponding property in the Defaults section.

The Format category contains several properties to control how the values are displayed. Most of these formatting options are discussed in detail in the section 'Default' :ref:`Pivot-Table_Contents` . 



**Explicit Identifiers - Format - Use Default Standard Format** 



If you have specified a Standard Format in the Default section, then each explicit identifier will use that Standard Format unless you override it for a specific identifier. You can override the default Standard Format in two ways:

1) Specify another Standard Format for the specific identifier, or

2) Set Use Default Standard Format to 'No', and then specify the individual formatting options Decimal Places, 1000 Separator, and/or Scientific Notation.

Please note that the options for Decimal Places, 1000 Separator, and Scientific Notation are not available if you have specified a (default) standard format.



**Explicit Identifiers - Is Hidden** 



With this property you can control whether the given Explicit Identifier should be hidden (or removed) from the Pivot Table. Because the value of this property can be another identifier from your model, it provides you with additional flexibility as to which identifiers are displayed in the Pivot Table.



**Explicit Identifiers - ReadOnly** 



With this property you can make sure that the end user cannot modify this explicit identifier. By entering a multi dimensional identifier for this property you can control the read only status for individual values of the identifier in the Pivot Table.



If the identifier is not updatable in the first place (because it has a definition in the model), setting this property will have no effect. If you leave it blank, the property will be inherited from the ReadOnly property in the Defaults section.



**Explicit Identifiers - Ignored Aggregators** 



With this property you can prevent certain aggregator types from being displayed for a specific identifier. For example, consider a pivot table that displays both sales data and temperature data over time (for a certain day). When the end-user adds aggregators, by default all values in the pivot table are subject to aggregation. However, summing temperature values over time does not make much sense (while summing sales data over time does). When you tell the pivot table to 'ignore' the "Sum" aggregator for the temperature identifier, the pivot table will not display any totals over temperature values (when the end-user adds a "Sum" aggregator).



**Explicit Identifiers - Colors - Background Color** 



With this property you can specify an alternative background color for the (individual) values of the identifier. If not specified, the background color of the Grid Area will be used. 



**Explicit Identifiers - Colors - Text Color** 



With this property you can specify an alternative text color for the (individual) values of the identifier. If not specified, the text color of the Grid Area will be used. 



**Explicit Identifiers - Colors - Use Colors for Updatable Entries Only** 



With this property you can control whether or not the specified background and text color for this explicit identifier are only applied to grid cells that correspond to an updatable entry. This property can be usefull to visually distinguish between the updatable and non-updatable cells in the pivot table.



**Explicit Identifiers - Tooltip Text** 



With this property you can specify your own text that will be used in the small (yellow) tooltip box that appears when you hover the mouse over the cells in the Pivot Table while it has the focus. You can enter a specific quoted string or a string parameter. If the resulting string contains the name of an index enclosed within two % characters, the Pivot Table will replace it with the current element for the specific cell (for example: "Transport from %fromCity% to %toCity%" may result in a tooltip "Transport from Amsterdam to The Hague"). Similarly if you include %case% in the string, it will be replaced by the corresponding case name in a multiple case view of the Pivot Table.



If you leave this property empty, then the Pivot Table will generate a tooltip text using the name of the identifier(, the case) and all relevant element names.



Please note that you can turn off the tooltip feature with the property Show Tooltips on the Grid Area tab.



**Explicit Identifiers - Procedures & Assertions - On Change** 



With this property you can specify a procedure that will be executed each time that the end user changes a value of the identifier in the Pivot Table. If you specify a procedure with element parameter arguments matching the indices in the domain of the identifier, you can determine which of the values of a multi dimensional identifier is changed. If not specified the corresponding property in the Defaults section is used.



**Explicit Identifiers - Procedures & Assertions - On Select** 



With this property you can specify a procedure that will be executed each time that the end user selects a cell corresponding to the current explicit identifier in the Pivot Table. If you specify a procedure with element parameter arguments matching the indices in the domain of the identifier, then the procedure will also be called if the end-user switches between cells belonging to the same identifier. If not specified the corresponding property in the Defaults section is used.



**Explicit Identifiers - Procedures & Assertions - On Double-Click** 



At this property you can specify a procedure that will execute each time that the end user double-clicks a cell corresponding to the current explicit identifier in the Pivot Table.  If you specify a procedure with element parameter arguments matching the indices in the domain of the identifier, you can determine which of the values of a multi dimensional identifier is double-clicked. If not specified the corresponding property in the Defaults section is used.



**Explicit Identifiers - Procedures & Assertions - Assertion (1-5)** 



You can specify up to 5 assertions that will be checked each time that you change a value of the corresponding identifier in the Pivot Table. For each assertion you can set its type to either 'immediate' (the default) or 'delayed'.  You can read more about using assertions in page objects :ref:`Shared-Object-Properties_Object_Properties_-_Assert` .



**Explicit Identifiers - Procedures & Assertions - Ignore Default Assertions** 



If you have specified any assertions in the 'Default' section, an additional property will appear for the explicit identifiers: Ignore Default Assertions. With this property you can control for a specific explicit identifier whether you want to use the 'default assertions + the explicit assertions' or ignore the default assertions and only use the explicit assertions (if any).




**Default** 



The properties in this category are used as the default properties for each identifier in the Pivot Table. The default properties are used for all identifiers for which no corresponding property has been specified in the Explicit section. Most of these properties (with the exception of the unit related properties in the default section) can also be specified by a model identifier. You can even use indexed identifiers as values for most default properties. However, properties specified by some indexed identifier A are only applicable to a specific (Explicit or Implicit) identifier B, whenever the domain of identifier A is a (permuted) subset of the domain of identifier B.



For example: if you have two identifiers in your table X(i,j) and Y(j,k), then a default background color that is specified using MyColor(i,j) will be used for the identifier X, but will be ignored for identifier Y. Similarly, a default background color specified using MyOtherColor(j) will be used for both identifiers.



In addition to indices that can be mapped onto the indices of the Explicit or Implicit Identifiers, you can also use an index in the set AllIdentifiers in the domain of a default property. For example: if you specify the background color using MyIdentifierColor(IndexAllIdentifiers), then for an identifier X the background color will be taken from the value MyIdentifierColor('X').



**Default - Format - Standard Format** 



If you want to use the same format for multiple identifiers and objects, then you can store the format settings in a 'standard format'. These standard formats can be selected and managed when you press the wizard button for this property.



**Default - Format - Decimal Places** 



Here you can specify the default number of decimal places to be used when displaying the numerical value. If you leave it empty (and also have not specified it for a specific identifier), then the Pivot Table will try to print as much significant decimals that fit within the current cell width. You can specify an (integer valued) identifier.



**Default - Format - Show 1000 Separator** 



This property determines whether or not a thousand separator should be displayed (1,000.00 vs. 1000.00). 



**Default - Format - Scientific Notation** 



This property determines when it is allowed to use a scientific notation.



**Default - Format - 0-1 Values** 



If you are only interested in seeing whether a value is at its default or not, you can use this property. If set to Yes, then all entries will be displayed as checkboxes. All non defaults are displayed as a checked checkbox instead of the actual value. Furthermore, the value can be changed from default to non-default (and vice versa) by (un)checking in the checkbox.



**Default - Format - Show Value Bar** 



This property allows you to display a small horizontal bar in the cells in the grid area, representing the numerical values. You can decide to




#.  	not show bars at all (default),
#.  	show a value bar instead of the number it represents, or
#.  	show a value plus the number it represents.



By default, all cells with a minimum value (with respect to the specific explicit identifier) will display no bar and all cells with a maximum value will display a bar that totally fill the cell. In case the minimum value is larger than zero, the value corresponding to the left border of the cell is reset to zero. To override this standard behavior the minimum and maximum values can also be specified explicitly.



**Default - Format - Value Bar Minimum** 



With this property you can specify the numerical value that corresponds to the left border of the cell.



**Default - Format - Value Bar Maximum** 



With this property you can specify the numerical value that corresponds to the right border of the cell.



**Default - Format - Show Default Values** 



Decides whether the default values of an identifier should be displayed explicitly or as a blank.



**Default - Format - Alignment** 



This property determines how the value is aligned horizontally within its cell. If not specified, numerical values will be right-aligned, all other values will be left-aligned.











