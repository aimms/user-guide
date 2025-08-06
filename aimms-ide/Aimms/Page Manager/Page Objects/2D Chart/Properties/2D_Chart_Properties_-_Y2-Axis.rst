

.. _2D-Chart_2D_Chart_Properties_-_Y2-Axis:


Y2-Axis
=======

**Description** 

The Y2-axis tab contains all properties needed to specify a second Y-axis (possibly with a different scale). This second Y-axis is displayed along the right side of the chart. The Y2-axis section is also a property that has two possible values: "Show" and "Don't show". If it is set to "Show", the second Y-axis will be displayed in the chart. Also, all other relevant properties for the Y2-axis will become visible in the tree. These relevant properties are:



**Hide axis, use Y-scale** 

This property allows you to hide the Y2-axis, but still display its associated data in the chart. If set to 1, the 'Scale/Minimum', 'Scale/Maximum' and 'Misc. Settings/Logarithmic' properties of the Y-axis are used, to ensure that the data displayed matches the scale of the Y-axis (which is the only axis displayed then). You might want to use this property if the value range of both your Y-axis data and your Y2-axis data are quite close to each other, which may make the actual Y2-axis a bit superfluous. By using the Y2-axis data however, you can display your data using two different chart types.



**Draw on top of Y-axis data** 

This property specifies whether Y2-axis identifier data will be drawn in front of Y-axis identifier data. If the property is set to 1, this is the case. Otherwise, the Y-axis identifier data will be drawn in front of the Y2-axis data.



**Chart type** 

This property specifies the chart type that is used for displaying the identifier data of the Y2-axis. Not all chart types that are possible on the Y-axis are allowed. The allowed Y2-axis chart types are "Plot", "Bar", "Stacking Bar", "Area", "High/Low", "High/Low Open/Close", "Candle" and "Bubble".



You can use the ``Y2ChartTypeConstants``  set in ``Chart2DconstantsModule`` .



**Identifier** 

This property is analogue to the 'identifier' subtree of the Y-axis.



See also: identifier subtree on the :ref:`2D-Chart_2D_Chart_Properties_-_Y-Axis`  



**Title** 

This property is analogue to the 'title' property of the Y-axis.



See also: title property on the :ref:`2D-Chart_2D_Chart_Properties_-_Y-Axis`  



**Annotation** 

The properties in the 'annotation' subtree of the Y2-axis are analogue to the corresponding properties in the Y-axis 'annotation' subtree.



See also: annotation subtree on the :ref:`2D-Chart_2D_Chart_Properties_-_Y-Axis`  



**Scale** 

The 'scale' subtree is partly analogue to the 'scale' subtree of the Y-axis. It has an additional node: Multiplier. When Multiplier is not equal to zero, the 'scale' subtree like the one of the Y-axis is not available, while a second node, Constant, is. The Multiplier and Constant can be used to scale the Y2-axis based on the scale of the Y-axis like: 'Y2-scale' = 'Y1-scale' * multiplier + constant. This can be used e.g. to display temperature in both degrees Celcius and Fahrenheit.



See also: scale subtree on the :ref:`2D-Chart_2D_Chart_Properties_-_Y-Axis`  



**Misc. settings** 

The 'misc. settings' subtree is analogue to the 'misc. settings' subtree of the Y-axis.



See also: misc. settings subtree on the :ref:`2D-Chart_2D_Chart_Properties_-_Y-Axis`  





