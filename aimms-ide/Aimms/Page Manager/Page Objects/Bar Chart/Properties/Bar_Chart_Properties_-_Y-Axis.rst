

.. _Bar-Chart_Bar_Chart_Properties_-_Y-Axis:


Y-Axis
======

**Description** 

On the Y-Axis property tab, you can specify the numerical range to be displayed along the Y-axis of a bar chart. By default, AIMMS determines the lower and upper bound of the range dynamically, using the current data in the chart. If these standard bounds are not appropriate, you can specify the lower and upper bound yourself. These bounds can be specified either by fixed values or via identifiers from the model. Besides the lower and upper bounds, you can also specify the number of grid points to be displayed.

If your chart contains multiple identifiers whose values are not in the same order of magnitude, you will get a bar chart with some very large bars and some very small bars. To adjust this, you can specify a scaling value for every identifier in the bar chart. These scaling values can either given as fixed numbers or via identifiers from the model.

It is also possible to specify a Base Line, which can be a value or a numerical identifier. When using a base line, the bars will not start at 0, but at the specified base line value. With this option you can visualize the differences from some (average) value.





