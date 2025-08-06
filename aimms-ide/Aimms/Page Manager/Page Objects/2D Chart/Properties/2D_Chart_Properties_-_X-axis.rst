

.. _2D-Chart_2D_Chart_Properties_-_X-axis:


X-axis
======

**Description** 

The X-axis tab contains a number of properties and property subtrees. With these properties, you can control all X-axis related settings of the 2D chart.



**Domain** 

The most important property of the X-axis tab, is the domain property. By setting this property, you can specify which values will be shown along the X-axis in your chart. The domain can be an index, a one-dimensional parameter or a one-dimensional string parameter. In case you specify a one-dimensional parameter, the X-axis values will be scaled according to the values of this parameter. For example, if you specify a parameter containing the values 1, 4 and 20, a scale of 0 to 20 will be shown along the X-axis. Should you have specified a string parameter with the values "1", "4" and "20" (or an index with values '1', '4' and '20'), only three equidistant values would have been shown along the X-axis.



**Unit** 

If the X-axis domain that you've specified has a unit assigned to it, you can specify an alternative unit through this property. The X-axis will be scaled accordingly.



Note that this property only appears in case you use a numeric parameter for the X-axis domain, since the two other possible X-axis domain types (i.e. a set or a string parameter) don't support units.



**Annotation** 

The X-axis tab contains an annotation subtree. In this subtree, the following properties can be set:



**Placement** 

This property controls where to place the axis annotation and the axis title. The allowed values are:



``Min`` 	 the annotation and title are placed just below the lowest Y-data value in your chart

``Max`` 	 the annotation and title are placed just above the highest Y-data value in your chart

``Origin`` the annotation and title are placed at the level of the Y-axis where the X-axis crosses it

``Auto`` 	 the object decides automatically where the annotation and title are best placed.	



You can use the ``AnnotationPlacementConstants``  set in ``Chart2DconstantsModule`` .



**Origin placement** 

This property controls where to draw the Y-axis on the X-axis. The allowed values are:



``Auto`` 	the object decides automatically where on the X-axis the Y-axis will be drawn

``Min`` 	the Y-axis is drawn at the far left of the X-axis

``Max`` 	the Y-axis is drawn at the far right of the X-axis

``Zero`` 	the Y-axis is drawn where the X-axis has value 0



You can use the ``AnnotationOriginPlacementConstants``  set in ``Chart2DconstantsModule`` .



**Rotation angle** 

This property specifies the angle, in degrees, at which the X-axis annotation is rotated. With large labels on the X-axis, a value of 90 degrees is a good choice.



**Show every n-th label** 

This property controls which labels are displayed along the X-axis. If you specify a value n, every n-th label will be printed. With this property, in combination with the number of first label shown property, you can control the X-axis annotation in a straightforward manner. If you need even more flexibility on which labels to display and which not, you may want to consider specifying a one-dimensional string parameter as the X-axis domain and assign it empty strings for the labels that you don't want to display.



**Number of first label shown** 

This property specified which label will be the first label shown. The first label of your X-axis domain has number 1.



**Precision** 

This property controls the number of decimals displayed in case of numeric X-axis labels. If you specify the value 0 or less, that value indicates the precision in powers of 10.



**Tick spacing** 

This property specifies the number of ticks displayed on the X-axis. If set to 1, every possible X-axis label gets a tick, if set to 2, every second possible X-axis label gets a tick, etc.



**Label spacing** 

In case you have specified a numeric parameter for the X-axis domain, you can control the spacing of the X-axis annotation labels with this property. You can set the (numerical) distance between successive labels.



**Y-Axis origin** 

With this property you have even finer control over the location of the Y-axis. You can specify the exact location (label) on the X-axis where the Y-axis should cross it.





**Scale** 

The scale subtree gives you control over the scaling of the X-axis. It has the following properties:



**Data minimum** 

This property specifies which data is displayed in your chart, with respect to the X-axis values of the data. For example, if your X-axis domain contains a one-dimensional parameter with values ranging from –10 to 10, and if you specify the value 0, your chart will only display data that has an X-value greater than or equal to 0.



**Data maximum** 

This property has the same meaning as the data minimum property, only here you specify the maximum X-axis value of the data to be displayed in your chart.



**Minimum** 

This property specifies the minimum value displayed along the X-axis. Even if no data with such an X-axis value exists.



**Maximum** 

This property specifies the maximum value displayed along the X-axis. Even if no data with such an X-axis value exists.



**Origin base** 

This property can only be specified for polar and (filled) radar charts. It specifies at what angle (in degrees) the Y-axis is located with respect to the X-axis.





**Gridlines** 

The gridlines subtree lets you control the displaying of X-axis gridlines. It contains the following properties:



**Spacing** 

This property determines the spacing between the individual gridlines. If set to 0, no gridlines are shown. In case of a radar chart, any non-zero value that you specify, will result in the same gridline distance (in radar charts, there is only one sensible way of drawing the X-axis gridlines).



**Show on top** 

If you set this property to 1, the gridlines appear in front of the chart. If you set it to 0 (the default), the gridlines appear behind the chart.





**Style** 

There is a subtree style under the gridlines subtree, that lets you control the appearance of the gridlines. It has the following three properties:



**Color** 

This property controls the color of the gridlines.



**Pattern** 

This property controls the pattern of the gridlines (e.g. solid, dotted, etc.).



You can use the ``LinePatternConstants``  set in ``Chart2DconstantsModule`` .



**Width** 

This property controls the width (i.e. the line thickness) of the individual gridlines.





**Misc. settings** 

The X-axis supports some more properties, that don't fall into one of the previous categories. Those properties are place in the misc. settings subtree:



**Title** 

With this property you can specify the title that should be displayed along the X-axis.



**Show unit in title** 

If there is a numerical identifier specified on the X-axis, which has a unit assigned to it, this unit can be displayed in the X-axis title. Set this property to 1 (the default) if you want this behavior, set it to 0 if you don't want the unit to be displayed in the title.



**Color** 

This property set the color of the X-axis, the X-axis labels and the X-axis title.



**Reversed** 

By setting this property to 1, you can reverse the order of the X-axis.



**Logarithmic** 

By setting this property to 1, the X-axis is shown on a logarithmic scale. This property doesn't have any effect on (stacked) bar charts.





