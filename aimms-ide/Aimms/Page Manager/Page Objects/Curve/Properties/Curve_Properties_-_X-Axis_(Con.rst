

.. _Curve_Curve_Properties_-_X-Axis_(Con:


X-Axis (Continuous)
===================

**Description** 

By default the range of the x-axis will be automatically calculated so that all data is visible. It is possible however to set the lower and upper bound of the x-axis. Be sure to activate the Horizontal Scroll Bar item if you want to be able to scroll along the x-axis using the mouse. If you don't do this, it is only possible to scroll by clicking on a point in the curve and using the left and right arrow keys (or tab key).

On the Y-Axis property tab, you can specify the numerical range to be displayed along the Y-axis of a Curve. By default, AIMMS determines the lower and upper bound of the range dynamically, using the current data in the curve. If these standard bounds are not appropriate, you can specify the lower and upper bound yourself. These bounds can be specified either by fixed values or via identifiers from the model. Besides the lower and upper bounds, you can also specify the number of grid points to be displayed.

If your curve contains multiple identifiers whose values are not in the same order of magnitude, you will get a Curve object with some lines displayed at the top side of the plot area, and some lines at the bottom side of the plot area, and these lines will look rather straight. To adjust this, you can specify a scaling value for every Y-axis identifier. These scaling values can either given as fixed numbers or via identifiers from the model.





