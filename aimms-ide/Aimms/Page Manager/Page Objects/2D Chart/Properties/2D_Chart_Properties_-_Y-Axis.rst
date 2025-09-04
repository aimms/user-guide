

.. _2D-Chart_2D_Chart_Properties_-_Y-Axis:


Y-Axis
======

**Description** 

On the Y-axis tab, all Y-axis related properties can be specified.



**Chart type** 

This property determines the chart type in which your data will be displayed. Certain chart types demand your data to satisfy one or more constraints. All individual chart types are mentioned below. You're advised to read the information for the identifier property first, before continuing.



You can use the ``YChartTypeConstants`` set in ``Chart2DconstantsModule``.



Plot

Chart type 'plot' (default) shows a plotted chart. You can either specify exactly one two-dimensional identifier, or at least one scalar or one-dimensional identifiers.



Bar

Chart type 'bar' shows your data in a bar chart. You can either specify exactly one two-dimensional identifier, or at least one scalar or one-dimensional identifiers.



Pie

Chart type 'pie' shows your data in one or more pie charts. The number of pie charts displayed is equal to the number of elements in the X-axis domain specified. The free index of every Y-identifier you specify, is displayed as one slice of each pie chart shown. There is one exception: if you don't specify an X-axis domain and only specify one one-dimensional Y-axis identifier, just one pie chart will be drawn, containing all elements of the index of the Y-axis identifier as slices of the chart. Please note that in all cases, only positive values are displayed as slices; negative values cannot be displayed.



Stacking bar

Chart type 'stacking bar' shows your data as a stacking bar chart. This layout is the same as a bar chart, the difference being that multiple bars belonging to one X-axis label are drawn on top of each other instead of next to each other. The stacking bar chart has the same data needs as the bar chart.



Area

Chart type 'area' shows your data as an area chart. This layout is basically a plot chart. The difference is that the area below the plotted line is filled with a color of choice.



High/Low

Chart type 'high/low' shows your data as a high/low-chart. This type of chart is used for displaying stock data. You should specify two Y-axis identifiers: the first containing the highest values of a stock and the second containing the lowest values of this stock.



High/Low Open/Close

Chart type 'high/low open/close' shows your data as a high/low open/close chart. This type of chart is also used for displaying stock data. Compared to the 'high/low' chart type, the opening and closing values of a stock are also displayed. The order in which the data must be supplied is Low/High/Open/Close. So, four one-dimensional Y-axis identifiers should be provided.



Candle

Chart type 'candle' shows your data as a candle chart. This type of chart is yet an other way of displaying stock data. The data to show should be in the same format as data for a 'high/low open/close' chart.



Polar

Chart type 'polar' shows your data as a polar chart. With a polar chart, you can display data that depends on a direction (in degrees). For the X-axis domain, you should specify an index or a parameter over the range 0 to 359. The circle around the polar chart is the X-axis.



Radar

Chart type 'radar' shows your data as a radar chart. With a radar chart, it's easy to compare a (small) number of data series on a number of values. For example, a radar chart would be an excellent choice for comparing the skills of three students in seven different subjects.



Filled radar

Chart type 'filled radar' is basically the same as chart type 'radar', only in a filled radar chart the area enclosed by the lines for the various data series is filled with a color of choice.



Bubble

Chart type 'bubble' shows your data as a bubble chart. In a bubble chart, you can plot an even number of Y(2)-axis identifiers. The odd-numbered identifiers determine the Y(2)-value of the lines in the chart, while the even-numbered ones determine the size of the symbols that are drawn on the lines. Please note that the appearance settings for a pair of identifiers should be set for the odd-numbered one. Any appearance setting specified for the even-numbered identifier(s) is ignored by the chart. If you specify a different legend entry for the odd- and the even-numbered identifier, a single legend entry is composed by separating both entries with a slash ('/') in the legend.





**Identifier** 

Together with the X-axis domain, the Y-axis identifier is the most important property of the 2D Chart ActiveX object. This is the property that specifies which data is displayed in the chart. You can specify either one two-dimensional parameter as the first identifier, or specify a series of scalar and/or one-dimensional parameters, by double-clicking on the 'new identifier' property to create a new identifier if needed.



The dimension of the first identifier is important. If it's a two-dimensional parameter, no further identifiers are allowed to be created. If it's a scalar or a one-dimensional parameter, you can create more identifiers if you like. Those cannot be two-dimensional parameters.



In the identifier subtree, more properties can be specified:



**Unit** 

If the identifier that you've specified has a unit assigned to it, you can specify an alternative unit through this property. The Y-axis will be scaled accordingly. Please be careful when you specify more than one identifier to be displayed on the Y-axis. For example, specifying two identifiers that represent surfaces in, say, m^2 and km^2 respectively, may result in an unwanted (though correct) scaling. Please also be careful when displaying identifiers that have units of different quantities assigned to it. AIMMS will display everything correctly, but the scaling may be not what you intended. When specifying identifiers that have units of different quantities, you should consider using the Y2-axis, which supports these situations better.



**Legend entry** 

With this property, you can specify what entry the legend should contain for the current identifier. If the current identifier is a two-dimensional parameter, the legend entry is ignored, since in such cases the legend will automatically be filled with the set elements corresponding to the identifier index that doesn't match the X-axis domain.



**Value label string** 

With this property, you can specify the string that should appear in the tooltip, when you click on a chart. You can enter either a literal (static) string, or a string parameter with a dimension that is smaller than or equal to the dimension of the corresponding Y-axis identifier. By using the AIMMS ``FormatString`` -function, this property offers the maximum in flexibility. You can, for example, show the value of the point that is clicked in the chart, in the format that you want. Consider for example a Y-axis identifier ``Dummy(i, j)``. If you define a string parameter ``ValueOfDummy(i, j)``, with definition ``FormatString("The current dummy value is %6.2n", Dummy(i, j))``, for every point that you click on in the chart, a nicely formatted string appears.



**Remove default values** 

With this property, you can override the remove all default values property under Y-axis/Misc. settings, for each Y-axis identifier. The property is only displayed in case the remove all default values property has the (non-default) value of 1. The remove default values properties all have a default value of 1, initially. This ensures that when the remove all defaults property is set to 1, all defaults are indeed removed from the chart. Setting a remove default values property of a certain Y-axis identifier to 0, has the effect that for that particular Y-axis identifier, the default values are still displayed.



**Appearance** 

With the properties in the (identifier) appearance subtree, you can customize the appearance of the chart element(s) that correspond to the current identifier. The following properties can be set, depending on the chart type (only the properties that are useful for the chosen chart type are displayed in the dialog):



**Fill/background color and Fill/foreground color** 

The fill background- and foreground color determine the colors of the current identifier in the chart. These properties can be of any dimension smaller than or equal to the dimension of the current identifier. To use a non-scalar color, use a non-scalar color parameter, i.e. an element parameter with range ``AllColors``.



**Fill/pattern** 

The fill pattern determines the pattern that is used to fill the representation of the current identifier in the chart. This property can be of any dimension smaller than or equal to the dimension of the current identifier. The property is available for the following chart types: bar, stacking bar, pie, area, candle and filled radar. The default value is "Solid".



You can use the ``FillPatternConstants`` set in ``Chart2DconstantsModule``.



**Line/color** 

This property determines the color of the line of the current identifier when the chart type is 'Plot'. The dimension of this property can be any dimension smaller than the dimension of the current identifier.



**Line/pattern** 

This property determines the pattern of the line in chart types where the current identifier is displayed as a line (e.g. in a 'Plot' chart). The default value is "Solid". The dimension of this property can be any dimension smaller than the dimension of the current identifier.



You can use the ``LinePatternConstants`` set in ``Chart2DconstantsModule``.



**Line/width** 

This property determines the width of the line in chart types where the current identifier is displayed as a line (e.g. in a 'Plot' chart). The default value is 1. The dimension of this property can be any dimension smaller than the dimension of the current identifier.



**Slice/offset** 

This property is only applicable in pie charts. It specifies the distance that a certain pie slice explodes from the pie chart.. The value to enter is a percentage of the pie radius. The default value is 0. The dimension of the property can be any dimension equal to or smaller than the current identifier.



**Symbol/color** 

This property determines the color of the symbols drawn at the data points in the chart, for the current identifier. The dimension of the property can be any dimension equal to or smaller than the current identifier.



**Symbol/shape** 

This property determines the shape of the symbols drawn at the data points in the chart, for the current identifier. The default value is "None", which means that no symbols are shown. The dimension of the property can be any dimension equal to or smaller than the current identifier.



You can use the ``SymbolShapeConstants`` set in ``Chart2DconstantsModule``.



**Symbol/size** 

This property determines the size of the symbols drawn at the data points in the chart, for the current identifier. The default value is 5. The dimension of the property can be any dimension equal to or smaller than the current identifier.



**Symbol image** 

This property only has effect when the symbol shape of the current identifier is set to "Image File". All the usual image properties can be set for the image shown at the data points in the chart.



For image properties, see property 'Backgroud image' on the :ref:`2D-Chart_2D_Chart_Properties_-_Display`  





**Title** 

This property specifies the title, displayed along the Y-axis.



**Rotation** 

If a title is specified for the Y-axis, a title rotation can also be entered. You can choose from the values "None", in which case the title is displayed horizontally above the Y-axis; "90 Degrees", in which case the title is rotated 90 degrees and displayed vertically along the left side of the Y-axis, or "270 Degrees", in which case the title is rotated 270 degrees and displayed vertically along the left side of the Y-axis.



You can use the ``TitleRotationConstants`` set in ``Chart2DconstantsModule``.





**Annotation** 

The Y-axis tab contains an annotation subtree. In this subtree, the following properties can be set:



**Placement** 

This property controls where to place the axis annotation and the axis title. The allowed values are:



``Min`` 	 the annotation and title are placed just before the first X-axis value in your chart

``Max`` 	 the annotation and title are placed just above the last X-axis value in your chart

``Origin`` the annotation and title are placed at the level of the X-axis value 0.

``Auto`` 	 the object decides automatically where the annotation and title are best placed.	



You can use the ``AnnotationPlacementConstants`` set in ``Chart2DconstantsModule``.



**Origin placement** 

This property controls where to draw the X-axis on the Y-axis. The allowed values are:



``Auto`` 	the object decides automatically where on the Y-axis the X-axis will be drawn

``Min`` 	the X-axis is drawn below the minimum Y-axis data value

``Max`` 	the X-axis is drawn above the maximum Y-axis data value

``Zero`` 	the X-axis is drawn where the Y-axis has value 0



You can use the ``AnnotationOriginPlacementConstants`` set in ``Chart2DconstantsModule``.



**Rotation angle** 

This property specifies the angle, in degrees, at which the Y-axis annotation is rotated.

 

**Precision** 

This property controls the number of decimals displayed in the Y-axis values. If you specify the value 0 or less, that value indicates the precision in powers of 10.



**Negative value color** 

With this property, you can specify the color that should be used for the Y-axis values that have a negative value. If you specify a color here, the minus sign in front of the values will not be displayed anymore. If you don't specify a color, the chart area foreground color, which is already used for the Y-axis value colors, will also be used for the negative values.



**Show thousand separators** 

Setting this property to 1 has the effect that the values along the Y-axis will display thousand separators (commas), if applicable.



**Tick spacing** 

This property specifies the numeric interval between every two ticks displayed on the Y-axis.

 

**Label spacing** 

You can control the spacing of the Y-axis annotation labels with this property. You can set the (numerical) distance between successive labels.



**Y-Axis origin** 

With this property you have even finer control over the location of the X-axis. You can specify the exact location (Y-axis data value) on the Y-axis where the X-axis should cross it.



See also: :ref:`2D-Chart_2D_Chart_Properties_-_X-axis`  





**Scale** 

The properties of the subtree 'scale' in the Y-axis tab have meanings analogue to the properties of the subtree 'scale' on the X-axis tab.



See also: :ref:`2D-Chart_2D_Chart_Properties_-_X-axis`  





**Gridlines** 

The properties of the subtree 'gridlines' in the Y-axis tab have meanings analogue to the properties of the subtree 'gridlines' on the X-axis tab.



See also: :ref:`2D-Chart_2D_Chart_Properties_-_X-axis`  





**Misc. Settings** 

The miscellaneous settings subtree on the Y-axis tab contains the following properties:



**Stacked** 

When you set the property 'Stacked' to 1, the data plots in the chart will be stacked upon each other. For example, consider a plot chart, with three identifiers displayed in it. For a certain x-value, the three identifiers have the values 1, 5 and 3 resp. Then the line of the first identifier will cross the y-axis at y-value 1 (just its value), the line of the second identifier at y-value 6 (= 1 + 5), and the line of the third identifier at y-value 9 (= 1 + 5 + 3).



**Logarithmic** 

Setting this property to '1' will show the Y-axis on a logarithmic scale.



**Scale axis to 100%** 

This property only affects stacking charts (i.e. charts of type 'Stacking Bar' or charts with property 'Stacked' set to 1). If set to 1, the Y-axis is scaled from 0 to 100%.



**Show identifier unit(s)** 

If you have specified identifiers which have units assigned to them to be displayed along the Y-axis, you can choose whether to display these units. In case all identifiers have the same unit assigned to them, the unit is appended to the Y-axis title. If the identifiers have different units, the unit of each individual identifier will be displayed in the legend. So, make sure you show the legend to see the units in the latter case.



The default value of this property is 1 (show the units), the other possible value is 0 (don't show the units).



**Remove all default values** 

This property, when set to 1, removes all default values that are displayed in the chart. For example, if an AIMMS identifier has default value of 0, all points that have a Y-value of 0 are removed from the chart. If you have specified more than one identifier on the Y-axis, all points are removed that have the default value of their corresponding AIMMS-identifier. So, if you display more than one AIMMS-identifier on the Y-axis, and those AIMMS-identifiers have different default values, setting this property to 1 removes all the default values of all displayed AIMMS-identifiers from the chart. However, this property can be overridden by the remove defaults property of each individual Y-axis identifier. 









