.. |img_def_default_property_bmp| image:: images/default_property.bmp


.. _Bar-Chart_Object_Properties_Colors:


Colors
======

**Description** 

Basically, for each object you can specify a color for:

*	Background.
*	Foreground (text and drawing lines).
*	Selection (the rectangle to indicate the users current selection).




**Color Scheme** 


In the bar chart, curve, parametric curve, and gantt chart object there is also a button available that allows you to specify the color scheme. In these objects the color scheme is used whenever the objects needs multiple colors to properly display its data. By default AIMMS use a color scheme that consists of the colors Blue, Yellow, Red, Green, Magenta, Cyan, Dark Grey, and Light Grey, but you specify your own color scheme.


If you click the button a dialog box will be opened in which you can (create and) select two types of Color Schemes: 


1.	Static Color Schemes, which you can freely extend and modify, and


2.	Subsets of AllColors, which are derived form all sets in your model that are a subset of the predefined set AllColors


Please note that the selected Color Scheme will be ignored if you specify an explicit color (or color parameter) as the identifier color. If you want to couple colors to specific elements of your identifier it is recommended to use indexed color parameter instead of a Color Scheme.








The specified foreground color will be used as the default for all identifiers in an object. Per identifier, and even per identifier element, you can specify an alternative color that overrules this default foreground color.





Specifying colors can be done via system colors (RGB-values), named user colors (defined in the project) and model colors (identifiers in the model). One of the advantages of model colors is that the color is based on the current value of an identifier, which you can change dynamically.





Tables, scalars, sparse lists, and composite tables have an additional property, Only updateable entries. If this options is checked, then the identifier specific color is only used for those entries that are updateable. The entries that are not updateable will get the standard foreground color.





**Note** 


Every newly created object initially uses a set of default colors for background, foreground and selection. You can set these default colors in the Color tab, using the small menu that appears when you press any of the |img_def_default_property_bmp| buttons. This menu contains two commands:

*	Set as **Default**: this will set the currently selected color as the default color (that is used when a new object is created).
*	Reset to **Default**: this will select the color that is currently used as default color.

*   For the data objects the Background color can be set to Transparent, in which case the underlying objects and/or background of the page will be shown as background.




**Learn more about** 

*	:ref:`Miscellaneous_System_Colors` 
*	:ref:`Miscellaneous_User_Colors` 
*	:ref:`Miscellaneous_Model_Colors` 



