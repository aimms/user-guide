

.. _Parametric-Curve_Curve_Properties_-_Curve:


Curve
=====

**Description** 

The Curve property tab contains the (parametric) curve specific properties. You can adjust the following properties here:



**Draw Lines** 

Initially AIMMS draws lines between the data points in a curve. When you turn this option off no lines will be drawn between the points.



**Fill Area** 

With this option you can indicate that the areas under a curve line should be filled with the color of the curve line itself. If the object displays multiple curve lines, this option could result in a display in which not all curves are clearly visible, because the filled area may obscure another line.



**Mark Points** 

When you choose this option the points that define the curve line will be marked. For different curves, different markers will be used.



**Line Width** 

This is the width of the curve lines between the points.



**Remove Defaults** 

When you choose remove defaults the set elements that have default values for each identifier in the object, are not shown.



**Swap Indices** 

If the curve object has a two-dimensional identifier as the Y-axis identifier (and there is a discrete X-axis), then by default, AIMMS will use the first free index to create the X-axis labels, and the remaining free index is used to draw individual curve lines. If you enable the option Swap Indices, this default usage of the free indices is reversed.



**Multiple Case Object** 

With the Multiple Case Object it is possible to show data from different cases in one object. This can not be done with two-dimensional identifiers. 



**Title** 

When you display only one scalar or one-dimensional identifier in the curve, you can chose to display a title. The default title is the name of the identifier that is displayed. Different titles can be defined in the text tab of the property window. In case of multiple identifiers, the titles can be displayed by using a legend.



**Legend** 

The legend shows which colors are used for identifiers or elements in the curve. 



**Y Labels** 

By turning this switch off, you remove the labels (numbers) from the y-axis. 



**X Labels** 

By turning this switch off, you remove the elements or the numbers from the x-axis.



**X Name** 

By turning this switch on, an identifier name will be shown under the x-axis. This identifier is either an index or a numerical parameter.



**Horizontal Scroll Bar** 

By default, the X-axis properties of the curve are such that all relevant data is directly visible in the curve. If you change these properties so that only a part of the curve is visible, then you can also choose to display a horizontal scroll bar.



**Vertical Scroll Bar** 

By default, the Y-axis properties of the curve are such that all relevant data is directly visible in the curve. If you change these properties so that only a part of the curve is visible, then you can add a vertical scroll bar to the curve, so that the user can scroll to other parts.



**Horizontal Grid** 

If you enable the horizontal grid, thin horizontal lines are drawn as a background of the curve for every grid point on the Y-axis. The number of grid points can be specified on the Y-Axis tab.



**Vertical Grid** 

If you enable the vertical grid, thin vertical lines are drawn as a background of the curve for every grid point on the X-axis. If the X-axis is discrete, the number of grid points corresponds to the number of elements shown. If the X-axis is continuous, you can specify the number of grid points on the X-Axis tab.



**Status Line** 

This options controls whether or not a status line is displayed. The status line is the area at the bottom of the object in which the value and description of the currently selected point is shown. If the Y-axis identifier is updatable the user can also change the value in this status line.



**Show Inactive Data** 

If this option is not selected, inactive data will be considered to have a default value. You can read more about inactive data in the Language Reference.



**Learn more about** 

*	:ref:`inactive_data`



