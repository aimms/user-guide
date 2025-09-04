

.. _2D-Chart_2D_Chart_Properties_-_Display:


Display
=======

**Description** 

The display tab contains all properties that influence the general appearance of the Chart2D ActiveX object. 



**Surrounding area** 

The 'surrounding area' subtree contains all properties needed to control the appearance of the area surrounding the actual chart area. Those properties are the following:



**Foreground color** 

The foreground color of the surrounding area is the default color of all objects drawn in the chart, for example the color of the axes and the axis annotation. The color of most objects in the chart can be overridden by setting the appropriate (foreground) color property. For example, to have most objects colored red, but the axes of the chart blue, set the surrounding area foreground color to red and the chart area foreground color to blue.



**Background color** 

The background color of the surrounding area is the background color of the Chart2D ActiveX object. This color again behaves as the default background color of the complete object, which can be overridden by setting the background color of specific objects/areas in the object.



**Background image** 

This property contains the filename of the background image to display in the surrounding area. Only .bmp image files are supported by the object.



**Background image layout** 

This property specifies the layout of the background image. Valid values are "Centered", "CropFitted", "Fitted", "Stretched", "StretchedToHeight", "StretchedToWidth" and "Tiled".



You can use the ``ImageLayoutConstants`` set in ``Chart2DconstantsModule``.



**Background image transparent** 

This property specifies whether the bitmap is displayed transparently. If so, any transparent areas in the bitmap are filled with the surrounding area background color. To display the image transparently, set this option to 1. Otherwise, specify value 0.



**Chart area** 

The chart area subtree contains all properties needed to control the appearance of the chart area. The settings you specify overrule the corresponding settings in the surrounding area subtree, but only for the actual chart area. So, for example, if you define a surrounding area background color of white and a chart area background color of green, the Chart2D ActiveX object will be a white rectangle, containing a smaller green rectangle. The properties that can be specified are the same as those of the surrounding area, plus the following:



**Chart area border type** 

This property determines the type of border to draw around the chart area. Possible values are "3D In", "3D Out", "Bevel", "Etched In", "Etched Out", "Frame In", "Frame Out", "None", "Plain" and "Shadow". Default is "None", i.e. no border.



You can use the ``BorderTypeConstants`` set in ``Chart2DconstantsModule``.



**Chart area border width** 

With this property, the border width can be specified. Valid values are 1 to 20, the default is 1.



**Margins** 

The margin subtree contains four properties, with which you can specify the margins around the chart area.



**Left** 

The left margin of the surrounding area, measured in pixels. The default value is 0, resulting in the largest possible space available for the chart.



**Right** 

The right margin of the surrounding area, measured in pixels. The default value is 0, resulting in the largest possible space available for the chart.



**Top** 

The top margin of the surrounding area, measured in pixels. The default value is 0, resulting in the largest possible space available for the chart.



**Bottom** 

The bottom margin of the surrounding area, measured in pixels. The default value is 0, resulting in the largest possible space available for the chart.



**3D view depth** 

Some chart types can be displayed in a 3D-look, such as bar charts. The 3D view depth specifies the chart depth as a percentage of the chart width. The values that can be entered are from 0 to 500.



**Elevation** 

This property specifies the elevation degree of the chart above the X-axis. Valid values are –45 to 45.



**Rotation** 

This property defines the rotation degree of the chart to the right of the Y-axis. Valid values are –45 to 45.



**Shading** 

This property defines the type of shading to be used in the 3D-like displaying of the chart. The possible values are "Color", "Dithered" and "None".



You can use the ``View3DShadingConstants`` set in ``Chart2DconstantsModule``.



**Misc. display settings** 

In the misc. display settings subtree, all other possible display-related properties can be set. The subtree contains the following properties:



**Show box around plot area** 

If this property is set to 1, a box is shown around the area in which the chart is plotted. If set to 0 (the default value), no such box is shown.



**Show chart horizontally** 

If this property is set to 1, the chart is shown horizontally, i.e. the X-axis and Y-axis are swapped. This can be quite useful with bar charts.



**Show outlines** 

If set to 1, outlines (contours) are drawn around chart objects like bars, pie slices, etc. If set to 0 (the default value), no outlines are drawn.



**Axis annotation font** 

This property determines the font that is used to display the annotation of all axes.



**Axis title font** 

This property determines the font that is used to display the titles along the axes.



**Click label subtree** 

The click label subtree contains properties that control the appearance of the little yellow label that is displayed when clicking somewhere in the chart. This label contains the data value of the point that is nearest to the point clicked.



**Hide value label on click** 

If this property is set to 0 (the default), a yellow label is displayed in a chart if you click in the chart with the left mouse button. The label shows the Y-value of the point that is closest to the mouse pointer when the mouse is clicked.



**Click label font** 

This property determines the font that is used to display the label that is shown when clicking the left mouse button in the chart.



**Click label decimals** 

This property specifies the number of decimals to use when displaying the Y-value in the click label. The default is 6. Allowed values range from 0 to 20.



**Show thousand separators** 

Setting this property to 1 has the effect that the values in the click label will display thousand separators (commas), if applicable.







