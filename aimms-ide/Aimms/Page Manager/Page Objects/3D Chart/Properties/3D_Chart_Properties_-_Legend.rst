

.. _3D-Chart_3D_Chart_Properties_-_Legend:


Legend
======

**Description** 

The legend tab contains all properties needed to show and customize the legend of the chart. Depending on the chosen chart type (surface, bar or scatter), you can manually control the labels of the legend or have the chart object automatically fill the labels. The Legend section itself is also a property that can contain one of the possible values "Show" and "Don't show". "Show" causes a legend to be shown (if the chart type provides this functionality), "Don't show" causes no legend to be shown.



You can use the ``ShowConstants`` set in ``Chart3DconstantsModule``.



**Title text** 

This property specifies the text to be used as the title of the legend area in the chart. For example, "Legend" is a title that can be used quite often.



**Labels** 

This property determines the labels that are displayed in the legend. In case the chart type is set to "Scatter", this property should be specified, in order to see a legend at all. The other two chart types allow the property to be specified, but in case you omit the property, the legend will be filled automatically. 



The property must be filled with a one-dimensional string parameter.



**Font** 

This property specifies the font that is used when displaying the legend area of the chart.



**Foreground color** 

This property specifies the foreground color of the text in the legend area.



**Background color** 

This property specifies the background color of the legend area.





**Background image** 

The filename of the image that should serve as a background in the legend area of the chart. The subproperties are the same as the usual image properties.



See also: background image properties on the :ref:`2D-Chart_2D_Chart_Properties_-_Display`  





**Border type/width** 

See: chart area border type and width on the :ref:`2D-Chart_2D_Chart_Properties_-_Display`  





**Misc. display settings** 

This subtree contains all other properties regarding the displaying of the legend. The properties are the following:



**Anchor** 

This property determines the location of the legend area, relative to the actual chart. The possible values are the 8 most common wind directions, e.g. "North", or "NorthEast".



You can use the ``LegendAnchorConstants`` set in ``Chart3DconstantsModule``.



**Orientation** 

This property determines the layout of the legend area. The two possible values are "Horizontal" and "Vertical" (default).



You can use the ``LegendOrientationConstants`` set in ``Chart3DconstantsModule``.



**Distribution range** 

This property is only displayed when the chart type is "Bar" or "Surface". It determines which entries will be shown in the legend. The possible values are "All" and "Data only". If you set the property to "All", the legend is filled with all entries that you've specified through the contour values. If you set the property to "Data only", the legend only shows those entries of the contour values that span the current data range.



You can use the ``LegendDistributionRangeConstants`` set in ``Chart3DconstantsModule``.



**Type** 

This property is only displayed when the chart type is "Bar" or "Surface". It determines the type of legend that is shown: either a continuous legend (value "Continuous") or a stepped (value "Stepped") can be displayed.



Notice that this property doesn't have any influence when the property IsShaded is set to 0. In that case, style "Stepped" is used.



You can use the ``LegendTypeConstants`` set in ``Chart3DconstantsModule``.



**Show every n-th label** 

This property is only displayed when the chart type is "Bar" or "Surface". With it, you can specify the labels that should be displayed in the legend. The default value is 1, indicating that every label should be present in the legend. If, for example, you set the value to 2, this means that every other label will be displayed in the legend.









