

.. _2D-Chart_2D_Chart_Properties_-_Legend:


Legend
======

**Description** 

The legend tab contains all properties needed to show and customize the legend of the chart. The legend entries that are shown can be set for each Y(2)-axis identifier on the Y(2)-axis tab. See property 'Legend entry'. The Legend section itself is also a property that can contain one of the possible values "Show" and "Don't show". "Show" causes a legend to be shown (if the chart type provides this functionality), "Don't show" causes no legend to be shown.



Notice that no legend is shown (even if you set the Legend property to "Show") if you use a scalar or a one-dimensional identifier and don't specify the legend entry property of the identifier.



You can use the ``ShowConstants``  set in ``Chart2DconstantsModule`` .



The available properties are the following:



**Title text** 

This property specifies the text to be used as the title of the legend area in the chart. For example, "Legend" is a title that can be used quite often.



**Font** 

This property specifies the font that is used when displaying the legend area of the chart.



**Horizontal alignment** 

This property specifies where exactly the footer is displayed below the chart. It can take the values of "Left", "Right" and "Center". "Center" is the default value. The horizontal alignment is relative to the chart area, not to the surrounding area. For example, if you have a legend displayed to the right of the chart area and you've specified "Right" as the horizontal alignment of the footer, the footer text is still completely displayed above the chart area and not aligned to the right of the chart object itself.



**Foreground color** 

This property specifies the foreground color of the text in the legend area.



**Background color** 

This property specified the background color of the legend area.



**Background image** 

The filename of the image that should serve as a background in the legend area of the chart. The subproperties are the same as the usual image properties.



See also: background image properties on the :ref:`2D-Chart_2D_Chart_Properties_-_Display`  



**Border type/width** 

See: chart area border type and width on the :ref:`2D-Chart_2D_Chart_Properties_-_Display`  





**Misc. display settings** 

This subtree contains all other properties regarding the displaying of the legend. The properties are the following:



**Anchor** 

This property determines the location of the legend area, relative to the actual chart. The possible values are the 8 most common wind directions, e.g. "North", or "NorthEast".



You can use the ``LegendAnchorConstants``  set in ``Chart2DconstantsModule`` .



**Orientation** 

This property determines the layout of the legend area. The two possible values are "Horizontal" and "Vertical" (default).



You can use the ``LegendOrientationConstants``  set in ``Chart2DconstantsModule`` .



**Reversed** 

Set this property to 1 to display all legend entries in the legend area in the reverse order.



**Use 3D-shading** 

This property only has effect when the chart is shown in a 3D-look (see: display tab/3D view depth). If the property is 1, the legend entries are also shown in a 3D-look.





