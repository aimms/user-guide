

.. _2D-Chart_2D_Chart_Properties_-_Style:


Style
=====

**Description** 

The "Style" tab contains some properties that are specific for certain chart types. The subtrees on this tab are therefore called after the chart type to which their properties apply.



**(Stacking) bar chart** 

The (Stacking) bar chart subtree contains the properties that are specific to the stacking bar chart and bar chart types.



**Cluster overlap** 

This property specifies the overlap between two bars in a (stacking) bar chart that share the same X-axis value, as a percentage of the bar's width. Valid values are from –100 to 100.



**Cluster width** 

This property specifies the with of a bar in a (stacking) bar chart, as a percentage of the available space for the bar. Valid values are from 0 to 100.





**Pie chart** 

The pie chart subtree contains the properties that are specific to the pie chart type.



**Sort order** 

This property specifies the order in which to sort the slices of a pie chart. The possible values are "Ascending", "Descending" and "None".



You can use the ``SortOrderConstants``  set in ``Chart2DconstantsModule`` .



**Threshold method** 

The 'Other' slice is the slice with 'rest values' that is frequently encountered in pie charts. For example, in a pie chart with election results, you can state that 50% of the people voted for candidate X, 33% for candidate Y, 15% for candidate Z and 2% for 'Other candidates'.



This property specifies the method used for determining the 'Other' slice. The possible values are "Cumulative cut-off percentage" and "Individual cut-off percentage". "Cumulative cut-off percentage" considers slices part of the 'Other' slice if the sum of their values is less than a certain percentage of the chart total, while "Individual cut-off percentage" considers slices part of the 'Other' slice if their individual values are less than a certain percentage of the chart total. The value that is used for determining the 'Other' slice is specified with the property 'Threshold value'.



Note that the "Minimum number of slices" property overrules the threshold method.



You can use the ``ThresholdMethodConstants``  set in ``Chart2DconstantsModule`` .



**Threshold value** 

This property is the value below which a slice is considered to be part of the 'Other' slice. See: threshold method.



**Minimum number of slices** 

This property specifies the minimum number of slices shown in the pie chart.

Note that this property overrules the threshold method.



**Start angle** 

This property specifies the start angle of the pie chart, i.e. the angle in the pie at which the first slice is drawn.





**Show percentages** 

The Show percentages subtree contains all properties that control whether and how the percentages of the individual slices of a pie chart are displayed.



**Show percentages** 

Selecting a value of 1 for this property has the effect that percentages will be shown for all individual slices in the pie chart. Additionally, it reveals the other properties available to control the display of the percentages. Please note that no percentages can be shown for the 'Other' slice (the third-party object used for implementing the 2D chart in AIMMS doesn't support this). Also note that in pie charts which display identifiers with negative values in it, the percentages are calculated over the positive values only, to prevent strange percentages from being displayed (no slices are displayed for negative values in pie charts).



**Display threshold** 

This property specifies the lowest percentage that should be shown in the pie chart. For example, setting this property to 5 will only show slice percentages that have a value of 5 or greater. The default value is 0, resulting in all percentages to be displayed.



**Number of decimals** 

This property controls the number of decimals that are displayed for the percentages. Specifying 0 will show no decimals at all. The default value is 1.



**Font** 

This property lets you select the font to be used for displaying the percentages.



**Foreground color** 

The foreground color of the percentages.



**Background color** 

The background color of the percentages.



**Border type** 

This property specifies the type of border that will be drawn around the percentages in the pie. The default value is "None", meaning no border at all.



**Width** 

This property specifies the width of the border to be displayed around the percentages.







**The 'other' slice** 

The 'other' slice subtree contains all properties that control the appearance of the 'Other' slice in a pie chart. The properties are:



**Fill background color** 

The background color of the 'other' slice.



**Fill foreground color** 

The foreground color of the 'other' slice.



**Label** 

This property specifies the text that appears in the legend for the 'other' slice.



**Slice style display** 

If this property is set to 0, the 'other' slice is not displayed. Instead, it is displayed as a 'bite' out of the pie chart. If set to 1, the 'other' slice is displayed just like the 'normal' slices.



**Offset** 

This property specifies the offset of the 'Other' slice. See: slice offset.





**High/Low Open/Close chart** 

The high/low open/close chart subtree contains the properties that are specific to the high/low open/close chart type.



**Show full width** 

If this property is set to 1, the open and close ticks are shown in their full width, i.e. on both sides of the vertical line. If set to 0 (the default), the open tick is shown on the left of the vertical line and the close tick on the right.



**Hide the open tick** 

If this property is set to 0 (the default), the open tick is shown. If set to 1, the open tick is not shown.



**Hide the close tick** 

If this property is set to 0 (the default), the close tick is shown. If set to 1, the close tick is not shown.





**Polar chart** 

The polar chart subtree contains the properties that are specific to the polar chart type.



**Allow negative Y-values** 

If this property is set to 1, and the data displayed contains negative Y-axis values, those values are also drawn. If the property is set to 0 (the default), any negative Y-axis values are ignored in the chart.



**Half range X-axis annotation** 

Set this property to 1 if the total X-axis range should be from –180 to 180 degrees. Set this property to 0 (the default) if the total X-axis range should be from 0 to 360 degrees.



**Bubble chart** 

The bubble chart subtree contains the properties that are specific to the bubble chart type.



**Bubble size method** 

With this property you can specify the method that is used for determining the size of the bubbles, relative to each other. The possible values are "Area" and "Diameter" (the default). When you specify "Diameter", the diameter of the bubble is sized proportionally to the value specified for the size (through every 2nd identifier), otherwise the area of the bubble is sized proportionally to that value.



**Minimum bubble size** 

The size of the bubble with the lowest corresponding data value in the bubble chart.



**Maximum bubble size** 

The size of the bubble with the highest corresponding data value in the bubble chart. Notice that the minimum bubble size doesn't necessarily have to be smaller than the maximum bubble size. Also notice that the bubble size isn't necessarily proportional to the data values: when you display values ranging from –10 to +10, the bubble corresponding to value 0 is not invisible, but, instead, a bubble of average size.



The number that you actually specify for the minimum/maximum bubble size has a different effect on the size, depending on the bubble size method specified. A value of 10 for the "Diameter" method shows a bubble of roughly the same size as a value of 1 for the "Area" method. This is due to the fact that the bubble size is a percentage relative to the complete chart area: 10% of the length ("Diameter") of the chart equals 1% of the area ("Area") of the chart.



