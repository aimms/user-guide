

.. _Network_Network_Object_Properties_-_Te:


Text
====

**Description** 

The network object has different text properties than other page objects. In the text tab of the network object you can specify for each node and arc which text is displayed and where this text should appear relative to the node/arc.



**Node/Arc** 

In this property field, the node or arc can be selected whose properties are to be shown or altered. For this selected identifier, you can choose to:

*	Show no text at all.
*	Show only the element names of the nodes (nodes only).
*	Specify other text, either via a quoted string or via a model identifier.




**Position** 


In the position property field, you can select the relative position of the text with respect to the node or arc.





For a node, you have 4 choices: at the Top, Left, Bottom or Right of the node. 





For an arc you have 2 choices: at the Left or at the Right of the arc. This left and right should be interpreted by 'looking in the direction of the arc'. So for example, if the arc points downwards, then 'Left' will result in the text being displayed at the right-side of the arc. Or if an horizontal arc points to the right, then 'Left' will result in the text being displayed above the arc. 





**Along Arc Slope**  


This property is only available for arcs, if you check this box then the text is not necessarily drawn horizontally, instead it is drawn using an angle that corresponds to the slope of the arc. 





**Text at Segment**  


This property is only available for arcs and only if the arc has the shape 2-Segments Line or 3-Segments Line (see :ref:`Network_Network_Object_Properties_-_Ar`  properties). With this property you can specify at which segment(s) the text will be displayed. 





**Tooltip Text**  


You can specify the text that should appear as a tooltip when you hover the mouse over either a node or an arc. The text can be specified as a literal quoted string or via a model identifier that may be indexed over the same indices that are used for the node or arc.





**Note** 

*	To make it easier to show flow values along the arcs, it is also allowed to choose parameters that are not string-valued. If you select a numerical identifier, its format can be adjusted in the Format tab of the Properties dialog box.



