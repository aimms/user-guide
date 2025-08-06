

.. _3D-Chart_3D_Chart_Properties_-_Z-Axis:


Z-Axis
======

**Description** 

The "Z-Axis" tab contains all Z-axis-related properties. On this tab, you can specify the actual parameters that you want to display in the 3D-chart.



**Identifier** 

In the identifier subtree, you can specify the identifier(s) that you want to display in the 3D-chart. The identifier(s) that you display may be scalar, one-, or two-dimensional.



A scalar identifier will lead to a flat surface to be displayed.

A one-dimensional identifier that you display, should depend on either the X- or the Y-axis domain.

A two-dimensional identifier that you display, should depend on both the X- and the Y-axis domain.



Note that only one identifier can be displayed at the same time, when the chart type is "Surface" or "Bar". In case of chart type "Scatter", more than one identifier can be displayed at the same time.



**Unit** 

In case the identifier(s) you show in your chart have a unit assigned to them, you can use this property to specify an alternative unit for each identifier. The Z-axis will be scaled accordingly.



**Remove default values** 

With this property, you can override the remove all default values property under Z-axis/Misc. settings, for each Z-axis identifier. The property is only displayed in case the remove all default values property has the (non-default) value of 1. The remove default values properties all have a default value of 1, initially. This ensures that when the remove all defaults property is set to 1, all defaults are indeed removed from the chart. Setting a remove default values property of a certain Z-axis identifier to 0, has the effect that for that particular Z-axis identifier, the default values are still displayed.



Please note that only the scatter chart type is able to display more than one Z-axis identifier simultaneously.





**Appearance** 

The appearance subtree is only displayed in case the chart type has been set to "Scatter". The subtree contains properties with which you can control the appearance of the different identifiers shown in the 3D scatter chart. The following properties can be set:



**Drop line / Color** 

This property determines the color of the drop lines for the current identifier. Of course, setting this property only has an effect if the property **Has drop lines**  on the display tab is set to '1'.



**Drop line / Pattern** 

This property determines the pattern of the drop lines for the current identifier. Of course, setting this property only has an effect if the property **Has drop lines**  on the display tab is set to '1'.



You can use the ``LinePatternConstants``  set in ``Chart3DconstantsModule`` .



**Drop lines / Width** 

This property determines the width of the drop lines for the current identifier. Of course, setting this property only has an effect if the property **Has drop lines**  on the display tab is set to '1'.



**Symbol / Color** 

This property determines the color of the symbol for the current identifier.



**Symbol / Shape** 

This property determines the shape of the symbol for the current identifier.



You can use the ``SymbolShapeConstants``  set in ``Chart3DconstantsModule`` .



**Symbol / Size** 

This property determines the size of the symbol for the current identifier.





**Gridlines** 

The gridlines subtree lets you control the displaying of Z-axis gridlines. It contains the following properties:



**Show on XZ-plane** 

Since in a 3D-chart gridlines for the Z-axis can be displayed in two planes (the XZ-plane and the YZ-plane), this property lets you specify whether the Z-axis gridlines should be shown on the XZ-plane. The default value is 0 (not shown), the other possible value is 1 (shown).



**Show on YZ-plane** 

Since in a 3D-chart gridlines for the Z-axis can be displayed in two planes (the XZ-plane and the YZ-plane), this property lets you specify whether the Z-axis gridlines should be shown on the YZ-plane. The default value is 0 (not shown), the other possible value is 1 (shown).



**Style** 

There is a subtree style under the gridlines subtree, that lets you control the appearance of the gridlines. It has the following three properties:



**Color** 

This property controls the color of the gridlines.



**Pattern** 

This property controls the pattern of the gridlines (e.g. solid, dotted, etc.).



You can use the ``LinePatternConstants``  set in ``Chart3DconstantsModule`` .



**Width** 

This property controls the width (i.e. the line thickness) of the individual gridlines.



**Misc. settings** 

The Z-axis supports some more properties, that don't fall into one of the previous categories. Those properties are placed in the misc. settings subtree:



**Title** 

With this property you can specify the title that should be displayed along the Z-axis.



**Hide axis** 

If you set this property to 1, the Z-axis will not be displayed anymore. If the property is set to 0 (the default), the Z-axis is displayed.



**Origin** 

This property is only available when the chart type is "Bar". It defines the Z-axis value from which bars are filled in a 3D bar chart.



**Show units** 

In case you have selected identifiers that have a unit assigned to them, you can use this property to specify whether or not to display the unit(s). In case you have specified identifiers that all have the same unit, the unit will be appended to the Z-axis title. In case you have specified identifiers with different units, the units will be shown in the legend for each individual identifier. Note that this latter case can only happen when the chart type is set to "Scatter", since this is the only chart type that supports more than one identifier to be actually displayed.



**Remove all default values** 

This property, when set to 1, removes all default values that are displayed in the chart. For example, if an AIMMS identifier has default value of 0, all points that have a Z-value of 0 are removed from the chart. If you have specified more than one identifier on the Z-axis, all points are removed that have the default value of their corresponding AIMMS-identifier. So, if you display more than one AIMMS-identifier on the Z-axis, and those AIMMS-identifiers have different default values, setting this property to 1 removes all the default values of all displayed AIMMS-identifiers from the chart. However, this property can be overridden by the remove defaults property of each individual Z-axis identifier.



Please note that only the scatter chart type is able to display more than one Z-axis identifier simultaneously.







