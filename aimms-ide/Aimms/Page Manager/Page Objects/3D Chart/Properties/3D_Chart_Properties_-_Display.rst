

.. _3D-Chart_3D_Chart_Properties_-_Display:


Display
=======

**Description** 

The display tab contains all properties that influence the general appearance of the Chart3D ActiveX object. 





**Surrounding area** 

The 'surrounding area' subtree contains all properties needed to control the appearance of the area surrounding the actual chart area. Those properties are the following:



**Foreground color** 

The foreground color of the surrounding area is the default color of all objects drawn in the chart, for example the color of the axes and the axis annotation. The color of most objects in the chart can be overridden by setting the appropriate (foreground) color property. For example, to have most objects colored red, but the axes of the chart blue, set the surrounding area foreground color to red and the chart area foreground color to blue.



**Background color** 

The background color of the surrounding area is the background color of the Chart3D ActiveX object. This color again behaves as the default background color of the complete object, which can be overridden by setting the background color of specific objects/areas in the object.



**Background image** 

This property contains the filename of the background image to display in the surrounding area. Only .bmp image files are supported by the object.



**Background image layout** 

This property specifies the layout of the background image. Valid values are "Centered", "CropFitted", "Fitted", "Stretched", "StretchedToHeight", "StretchedToWidth" and "Tiled".



You can use the ``ImageLayoutConstants``  set in ``Chart3DconstantsModule`` .



**Background image transparent** 

This property specifies whether the bitmap is displayed transparently. If so, any transparent areas in the bitmap are filled with the surrounding area background color. To display the image transparently, set this option to 1. Otherwise, specify value 0.





**Chart area** 

The chart area subtree contains all properties needed to control the appearance of the chart area. The settings you specify overrule the corresponding settings in the surrounding area subtree, but only for the actual chart area. So, for example, if you define a surrounding area background color of white and a chart area background color of green, the Chart 3D ActiveX object will be a white rectangle, containing a smaller green rectangle. The properties that can be specified are the same as those of the surrounding area, plus the following:



**Chart area border type** 

This property determines the type of border to draw around the chart area. Possible values are "3D In", "3D Out", "Bevel", "Etched In", "Etched Out", "Frame In", "Frame Out", "None", "Plain" and "Shadow". Default is "None", i.e. no border.



You can use the ``BorderTypeConstants``  set in ``Chart3DconstantsModule`` .



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





**Plot area** 

The plot area of a 3D chart object is the area in which the actual chart is drawn, e.g. the so-called "plot cube". It lies within the chart area.



**Background color** 

By default, the background color of the plot area is the same as the background color of the chart area (if specified, otherwise the background color of the surrounding area is used). With this property, you can override this default background color with the color of your choice.





**Floor subtree** 

The floor subtree can only be specified when the chart type is "Surface". It has the following two properties:



**IsZoned** 

If you set this property to 1, zones will be drawn on the floor of the plot cube. If this property is 0, its default value, no zones will be drawn on the floor of the plot cube.



**IsContoured** 

If you set this property to 1, contours will be drawn on the floor of the plot cube. If this property is 0, its default value, no contours will be drawn on the floor of the plot cube.





**Ceiling** 

The ceiling subtree can only be specified when the chart type is "Surface". It has the following two properties:



**IsZoned** 

If you set this property to 1, zones will be drawn on the ceiling of the plot cube. If this property is 0, its default value, no zones will be drawn on the ceiling of the plot cube.



**IsContoured** 

If you set this property to 1, contours will be drawn on the ceiling of the plot cube. If this property is 0, its default value, no contours will be drawn on the ceiling of the plot cube.





**Scaling** 

The scaling subtree contains properties that control the scaling of the plot cube. The following two properties exist:



**X-Scale (%)** 

This property sets the amount of scaling in the X-axis direction, measured as a percentage of the height of the cube. Values from greater than or equal to 0 are accepted.



**Y-Scale (%)** 

This property sets the amount of scaling in the Y-axis direction, measured as a percentage of the height of the cube. Values from greater than or equal to 0 are accepted.





**3D View properties** 

With the properties in the 3D view properties subtree, the 3D-appearance of the whole plot cube can be controlled. The following properties can be set:



**Perspective** 

With this property, you can control the perspective effect of the chart displayed. The value entered must be greater than 0. The perspective effect is reduced with higher values: in such cases a parallel projection is approached.



**X-rotation** 

This property specifies the number of degrees of rotation of the chart, in a counter-clockwise direction about the X-axis. The chart applies any rotations in the order Z-Y-X.



**Y-rotation** 

This property specifies the number of degrees of rotation of the chart, in a counter-clockwise direction about the Y-axis. The chart applies any rotations in the order Z-Y-X.



**Z-rotation** 

This property specifies the number of degrees of rotation of the chart, in a counter-clockwise direction about the Z-axis. The chart applies any rotations in the order Z-Y-X.





**Misc. display settings** 

This subtree contains some display-related properties that don't fall into one of the other categories.



**Axis font** 

This property determines the font in which the axis titles are displayed.



**Font rotation** 

This property determines the rotation applied to the axis annotation and titles. Possible values are "2D", "3D" and "None", "None" being the most readable option, "3D" the most 3D-like option.



You can use the ``FontRotationConstants``  set in ``Chart3DconstantsModule`` .



**Preview method** 

This property controls the way that the plot cube is displayed when rotating it. To rotate the plot cube, make sure the page is not in edit-mode, click on the plot cube with both mouse buttons at the same time, and finally move the mouse to see the rotation.



The property has the two possible values: "Full" and "Cube". "Full" will display the entire plot cube when rotating it, while "Cube" will only display the frame around the plot cube when rotating it. Use the "Cube" setting when you observe the "Full" setting to be slowing down the rotation process.



You can use the ``PreviewMethodConstants``  set in ``Chart3DconstantsModule`` .





**Click label subtree** 

The click label subtree contains properties that control the appearance of the little yellow label that is displayed when clicking somewhere in the chart. This label contains the data value of the point that is nearest to the point clicked.



**Hide value label on click** 

If this property is set to 0 (the default), a yellow label is displayed in a chart if you click in the chart with the left mouse button. The label shows the Z-value of the point that is closest to the mouse pointer when the mouse is clicked.



**Click label font** 

This property determines the font that is used to display the label that is shown when clicking the left mouse button in the chart.



**Click label decimals** 

This property specifies the number of decimals to use when displaying the Z-value in the click label. The default is 6. Allowed values range from 0 to 20.



**Show thousand separators** 

Setting this property to 1 has the effect that the values in the click label will display thousand separators (commas), if applicable.





**Chart style** 

This subtree contains all properties that control the style of the chart.



**Chart type** 

With this property, you can set the type of chart displayed. Valid values are "Bar", "Scatter" and "Surface".



The scatter chart is the only chart that supports the actual displaying of more than one identifier. However, if you specify one of the other two chart types, it is still possible to specify more than one identifier for the Z-axis. This is allowed in order to let you easily switch between the various chart types, without having to delete and/or redefine your identifiers over and over again.

 

You can use the ``ChartTypeConstants``  set in ``Chart3DconstantsModule`` .



**Has drop lines** 

This property is only displayed in case the chart type has been set to "Scatter". If set to 1, drop lines are shown for each point in the 3D scatter chart.



**Is transparent** 

Setting this property to 1 makes the chart transparent, so that objects otherwise hidden by the actual chart become visible.



**Is meshed** 

Setting this property to 1 will have the effect that so-called mesh-lines are drawn on a surface or bar chart. The default value is 1, the other allowed value is 0.



Note that at least one of the properties Is Meshed, Is Shaded, Is Contoured and Is Zoned should be set to 1 in order to show a chart at all. If all are set to 0, nothing is displayed.



**Top color** 

When you set the 'Is meshed' property to 1, the top color property becomes visible. This property specifies the color of the mesh-lines that appear in the chart for Z-values greater than the Z-axis origin value for bar charts. For surface charts, it specifies the color of the mesh-lines when looked upon from above.



**Bottom color** 

When you set the 'Is meshed' property to 1, the bottom color property becomes visible. This property specifies the color of the mesh-lines that appear in the chart for Z-values smaller than the Z-axis origin value. For surface charts, it specifies the color of the mesh-lines when looked upon from below.



**Is shaded** 

Setting this property to 1 will have the effect that a shade is drawn on a surface or bar chart.



Note that at least one of the properties Is Meshed, Is Shaded, Is Contoured and Is Zoned should be set to 1 in order to show a chart at all. If all are set to 0, nothing is displayed.



**Top color** 

When you set the 'Is shaded' property to 1, the top color property becomes visible. This property specifies the color of the shading that appears in the chart for Z-values greater than 0 for bar charts. For surface charts, it specifies the color of the shading when looked upon from above.



**Bottom color** 

When you set the 'Is shaded' property to 1, the bottom color property becomes visible. This property specifies the color of the shading that appears in the chart for Z-values smaller than 0 for bar charts. For surface charts, it specifies the color of the shading when looked upon from above.





**Is contoured** 

This property determines whether the chart has contour lines drawn on it.



Note that at least one of the properties Is Meshed, Is Shaded, Is Contoured and Is Zoned should be set to 1 in order to show a chart at all. If all are set to 0, nothing is displayed.



**Contour values** 

This property is needed to specify which contour values will be used in the 3D chart for creating contours or zones. A one-dimensional parameter is expected. This parameter should be filled with values that correspond to Z-axis values for which contour lines should be drawn on the bar or surface chart.



**Styles** 

The styles subtree contains properties that specify how the contours and zones on the bar and surface charts look. It contains the following properties:



**Fill / Color scheme** 

With this property, you can choose between two ways of associating colors with contour values. The two possible choices are "Fluent" (default) and "User-defined".



When you choose "Fluent", you can specify a color for the lowest contour level and a color for the highest contour level. AIMMS will calculate a fluent color scheme for the intermediate contour values. One color per contour value is generated, so the more contour values you specify, the more fluent the color scheme will be.



When you choose "User-defined", you can specify a one-dimensional color parameter and one extra color for the highest contour value (see properties below).



**Fill / Low level color** 

This property can only be specified when the color scheme is set to "Fluent". It specifies the color to be associated with the lowest contour value.



**Fill / High level color** 

This property can only be specified when the color scheme is set to "Fluent". It specifies the color to be associated with the highest contour value.



**Fill / color** 

This property can only be specified when the color scheme is set to "User-defined".

The contour fill color property lets you specify exactly what colors to use for the contouring of the chart. A one-dimensional color parameter (an element parameter with range ``AllColors`` ) is expected. The easiest way of doing this, is to create a one-dimensional color parameter over the same index as you used for the contour values property's one-dimensional parameter.



**Fill / highest level color** 

This property can only be specified when the color scheme is set to "User-defined".

Since specifying n contour values means creating n + 1 regions divided by the contour lines, you'll need one extra color on top of the color specified through the fill/color property. This property lets you supply this extra color. The color specified is used for coloring the region of Z-values higher than the last specified contour value.



**Line / color** 

This property specifies the color of the contour lines.



**Line / pattern** 

This property specifies the pattern of the contour lines.



You can use the ``LinePatternConstants``  set in ``Chart3DconstantsModule`` .



**Line / width** 

This property specifies the width of the contour lines.





**Is zoned** 

Set this property to 1 if you want to use zone regions in your chart. Those regions can be filled with various colors, to increase the readability of your chart. The property is used in conjunction with the contour values and colors.



Note that at least one of the properties Is Meshed, Is Shaded, Is Contoured and Is Zoned should be set to 1 in order to show a chart at all. If all are set to 0, nothing is displayed.



**Zoning method** 

This property controls the method used for zoning. Possible values are "Cells" and "Contours", for cell zoning resp. contours zoning.



You can use the ``ZoneMethodConstants``  set in ``Chart3DconstantsModule`` .



