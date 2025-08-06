

.. _Composite-Table_Object_Properties_-_Format:


Format
======

**Description** 

On the Format tab you specify how the values of an identifier are displayed in the object. For each numerical identifier you can specify:

*	The width (the maximal number of positions, including a decimal point, that the value may occupy).
*	The number of decimals.
*	Whether or not a thousand separator should be displayed (1,000.00 vs. 1000.00).
*	When it is allowed to use a scientific notation.




For non-numerical identifiers you can only specify the width.





If you want to use the same format for multiple identifiers and objects, then you can store the four settings above in a 'standard format'. These standard formats can be selected and managed from within this Format tab.


In addition to the format properties described above you can set some extra options:





**Show Defaults** 


Decides whether the default values of an identifier should be displayed or left blank. When creating an object, AIMMS automatically enables this option if the default value of an identifier is not equal to 0.





**Zero/One Values** 


If you are less interested in the specific value of an identifier, but merely want to show whether a value is zero or not, you can use this option. Any value not equal to 0 is then indicated by an 'x', and all values equal to 0 are left blank. When displaying subsets in a table, this style is automatically chosen by AIMMS. In this mode, the user can then toggle the value from 0 to 1 by double clicking on the entry. Note that this setting is not available for the composite table.





**Alignment** 


With the alignment option you can define how a value should be aligned within a given area. You can choose between left, centered, or right alignment. By default, AIMMS uses right alignment for numerical values, and left alignment for string values.





**# Decimals from Symbol** 


In addition to the statically defined number of decimals above, you can choose to let the number of decimals in the format depend on the value of an (integer valued) model identifier. If you specify this identifier, the static number of decimals that you defined above, is used as a maximum for the number of decimals. You can enter a scalar identifier, so that you can modify the number of decimals for the entire displayed identifier at once, but you can also enter a multi-dimensional identifier with a domain that matches the displayed identifier. In the latter case, you are able to specify a specific number of decimals for each individual element of the displayed identifier.





**Use Element Auto-complete List** 


If a scalar object is displaying an element parameter, an auto-complete dropdown list pops up during editing. You can switch off this auto-complete dropdown list by unchecking Use Element Auto-Complete List.





**Tips & Tricks** 

*	Standard formats can be used to make it possible to change the formats in different objects at the same time. For example, it is possible to introduce a 'table format', which you can use in all tables. In this way, it is later possible to change the formats in all tables without having to go through your whole project.



