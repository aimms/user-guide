

.. _Bar-Chart_Bar_Chart_Properties_-_Bar_Cha:


Bar Chart
=========

**Description** 

The Bar Chart property tab contains the bar chart specific properties. You can adjust the following properties here:



**Bar Spacing percentage** 

This value defines the distance between every two (groups of) bars as a percentage of the width of a bar. 



**Overlapping/Stacking Bars** 

When you use a bar chart to display two-dimensional data, you can choose whether the second dimension is displayed by grouping (partially overlapping) or by stacking the bars. If you choose for overlapping bars, then you can additionally specify the amount of overlap as a percentage of the bar width.



**Remove Default Elements** 

With this option you can indicate whether set elements for which only default values exist, should be displayed in the bar chart. You can use it to effectively reduce the width of a bar chart (or of a group of overlapping bars) when there are several of such elements. 



**Swap Indices** 

Initially AIMMS determines which dimension is shown along the x-axis, and which dimension is shown grouped/stacked. With this option you can swap the behavior of either dimension. For one-dimensional data, swapping the indices allows you to display the data as a single group of overlapping or stacked bars.



**Multiple Case Object** 

In a bar chart you can either display data from the (single) current case, or from the current multiple case selection. If no multiple cases have been selected, the data of the current case will be displayed. Because a multiple case display adds one dimension to the bar chart, you can only display multiple case data for a one-dimensional bar chart. 



**Fill Style** 

The fill style determines how the interior of the bars is drawn. You can select a pattern, a color, both or neither. If you want to specify your own colors for the bars, you can do so via the Color tab. 



**Title** 

If the bar chart contains only a single identifier, you can check this option to indicate that the name of the identifier (or its associated text) should be used as the title of the bar chart. The associated text can be defined in the Text tab of the Properties dialog box.



**Legend** 

When you have two-dimensional data in a bar chart, the elements associated with the second dimension will be displayed by stacking or grouping bars for every element along the x-axis. A color is associated with each element in the second dimension. You can show a legend above the bar chart, where a title is associated with each color. You can change the contents of a title in the Text tab of the Properties dialog box.



**Y Labels** 

With this option you can select whether you want to display the labels at the y-axis in the bar chart. 



**X Labels** 

With this option you can select whether you want to display the labels at the x-axis in the bar chart. 



**X Name** 

With this option you can select whether you want to display a name below the x-axis in the bar chart.



**Horizontal Scroll Bar** 

You can use the horizontal scroll bar in combination with the option to fix the number of labels that are shown on the x-axis. The default setting is that all labels are shown, in which case there is no need for a horizontal scroll bar.



**Vertical Scroll Bar** 

You can use the vertical scroll bar in combination with the option to set the range of the y-axis. The default setting is that the range of the y-axis is so that all bars can be seen in which case there is no need for a vertical scroll bar.



**Horizontal Grid** 

You can activate a horizontal grid to make the difference in height between bars more clear. You can define the number of grid lines in the y-axis tab of the bar chart property window.



**Vertical Grid** 

With this option you can select whether you want to display vertical grid lines between each two x-labels in the bar chart.



**Status Line** 

This options controls whether or not a status line is displayed. The status line is the area at the bottom of the object in which the value and description of the currently selected point is shown. If the status line is not displayed, it is still possible to change a value by pointing the mouse to the top of a bar and dragging it up or down.



**Show Inactive Data** 

If this option is not selected, inactive data will be considered to have a default value. In a bar chart this means that there are no bars drawn for the inactive data elements (assuming that the default of the identifier is 0). You can read more about inactive data in the Language Reference.



**Tips & Tricks** 

*	If you show only a scalar identifier in a bar chart and you remove all items, you can use the bar chart to indicate the level in a tank.




**Learn more about** 

*	:ref:`Bar-Chart_Object_Properties_-_Text`  
*	 Search for Inactive data (Language Reference) 



