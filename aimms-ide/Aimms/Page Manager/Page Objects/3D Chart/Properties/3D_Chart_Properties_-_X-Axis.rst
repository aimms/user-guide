

.. _3D-Chart_3D_Chart_Properties_-_X-Axis:


X-Axis
======

**Description** 

The X-axis tab contains a number of properties and property subtrees. With these properties, you can control all X-axis related settings of the chart.



**Domain** 

The most important property of the X-axis tab, is the domain property. By setting this property, you can specify which values will be shown along the X-axis in your chart. The domain can be an index, a one-dimensional parameter or a one-dimensional string parameter. In case you specify a one-dimensional parameter, the X-axis values will be scaled according to the values of this parameter. For example, if you specify a parameter containing the values 1, 4 and 20, a scale of 0 to 20 will be shown along the X-axis. Should you have specified a string parameter with the values "1", "4" and "20" (or an index with values '1', '4' and '20'), only three equidistant values would have been shown along the X-axis.



**Unit** 

If the X-axis domain that you've specified has a unit assigned to it, you can specify an alternative unit through this property. The X-axis will be scaled accordingly.



Note that this property only appears in case you use a numeric parameter for the X-axis domain, since the two other possible X-axis domain types (i.e. a set or a string parameter) don't support units.





**Annotation** 

The X-axis tab contains an annotation subtree. In this subtree, the following properties can be set:



**Show every n-th label** 

This property controls which labels are displayed along the X-axis. If you specify a value n, every n-th label will be printed. With this property, in combination with the number of first label shown property, you can control the X-axis annotation is a straightforward manner. If you need even more flexibility on which labels to display and which not, you may want to consider specifying a one-dimensional string parameter as the X-axis domain and assign it empty strings for the labels that you don't want to display.



**Number of first label shown** 

This property specifies which label will be the first label shown. The first label of your X-axis domain has number 1.





**Gridlines** 

The gridlines subtree lets you control the displaying of X-axis gridlines. It contains the following properties:



**Show on XY-plane** 

Since in a 3D-chart gridlines for the X-axis can be displayed in two planes (the XY-plane and the XZ-plane), this property lets you specify whether the X-axis gridlines should be shown on the XY-plane. The default value is 0 (not shown), the other possible value is 1 (shown).



**Show on XZ-plane** 

Since in a 3D-chart gridlines for the X-axis can be displayed in two planes (the XY-plane and the XZ-plane), this property lets you specify whether the X-axis gridlines should be shown on the XZ-plane. The default value is 0 (not shown), the other possible value is 1 (shown).



**Style** 

There is a subtree style under the gridlines subtree, that lets you control the appearance of the gridlines. It has the following three properties:



**Color** 

This property controls the color of the gridlines.



**Pattern** 

This property controls the pattern of the gridlines (e.g. solid, dotted, etc.).



You can use the ``LinePatternConstants`` set in ``Chart3DconstantsModule``.



**Width** 

This property controls the width (i.e. the line thickness) of the individual gridlines.





**Misc. settings** 

The X-axis supports some more properties, that don't fall into one of the previous categories. Those properties are placed in the misc. settings subtree:



**Title** 

With this property you can specify the title to display along the X-axis.



**Show unit in title** 

If there is a numerical identifier specified on the X-axis, which has a unit assigned to it, this unit can be displayed in the X-axis title. Set this property to 1 (the default) if you want this behavior, set it to 0 if you don't want the unit to be displayed in the title.



**Hide axis** 

If you set this property to 1, the X-axis will not be displayed. If the property is set to 0 (the default), the X-axis is displayed.





