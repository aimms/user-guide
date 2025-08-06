

.. _Network_Network_Object_Properties_-_Ar:


Arcs
====

**Description** 

In the arcs tab of the network property dialog box, various fields concerning arcs can be set.



**Arc** 

In the arc field, the arc in the network object whose properties are displayed is selected. If your network contains multiple arc identifiers, then you should select the arc that you want to modify here.



**Size** 

The size determines the thickness of an individual arc. This can be a value, a scalar identifier or a 2-dimensional identifier, indexed over the node sets. In this last case you can assign individual sizes for each arc. 



**Size of 1.0 equal to** 

Here you specify how the size of an arc is translated into pixels on the screen. There are two options:

*	Direct translation to pixels, which is independent of the current scale of the visible area.
*	Translated to coordinate points. This means that a size of 1 is measured as an interval of 1 along the current X-axis. For example, if the left side of the visible area is currently equal to 0 and the right side equal to 10, then a size of 1 is displayed as 1/10th of the total object width. In this mode the thickness of arcs will thus change if you zoom in or out.




**Size Limit** 


These property fields are limits on the sizes that can be specified. These limits are defined in pixels. A minimum and maximum size is specified, and arcs are never displayed thinner than the minimum size, and never thicker than the maximum size.





**Shape** 


The Network object offers 4 types of Arc Shapes:


1.	Straight Lines


2.	Curved Lines


3.	2-Segments Line (connecting two nodes via 1 horizontal and 1 vertical line)


4.	3-Segments Line (connecting two nodes via a horizontal-vertical-horizontal line or vertical-horizontal-vertical)


For each shape a number of properties can be set:





**Arcs as Arrows** 


If you check this box, then each arc is drawn with an arrow head pointing in the direction of the arc. By default, this arrow head is drawn at the middle of the arc (at 50%), but you can specify another percentage. This percentage can be a fixed value or an identifier, optionally indexed over the node sets.


If you have selected a 2- or 3-Segments Line as the Arc Shape, then you can also indicate on which individual segments you want to display the arrow head. The same percentage will be used for each selected segment.





**1st Segment** 


If you have selected a 2- or 3-Segments Line as the Arc Shape, then this property indicates whether the first segment is drawn horizontally or vertically. What the first segment is, depends on the direction of the Arc.





**Position of 2nd Segment** 


If you have selected a 3-Segments Line as the Arc Shape, then this property gives the percentage at which the second segment will start. If the first segment is drawn horizontally, then the (vertical) second segments will be drawn at the indicates percentage of the total horizontal distance between the from and to node. The default value for this position is 50%. This percentage can be a fixed value or an identifier, optionally indexed over the node sets.





**Curve Factor** 


If you have selected a Curved Line as the Arc Shape, then this property indicates the measure of curvature. A value of 0 will result in a straight line, while a value of 100 or -100 will result in a maximum curvature. With the sign of this factor you can specify whether the curved line is to the right or to the left of the connecting straight line between the nodes. This value can be a fixed value or an identifier, optionally indexed over the node sets.





**Selectable** 


With the properties in the Selectable group you can specify whether the user can select an arc by clicking on it.


By default an Arc is selectable. If you don't want an Arc to be selectable you can speficy a value equal to 0. This value can be a fixed value or an identifier, optionally indexed over the node sets.





You can specify where on the Arc a user should click to select it:


1.	Click on Arrow Head, this option is only available if the Arcs as Arrows is checked.


2.	Click on Grip Point, if this option is selected, special small points are drawn on top of each arc, in which the user can click. The position of these points is indicates by a percentage (default 50%). This percentage can be a fixed value or an identifier, optionally indexed over the node sets.


3.	Click on Entire Arc, this option is not available for the arc shape Curved Lines.


 





**Tips & Tricks** 

*	For the thickness of arcs it is possible to use a 2-dimensional parameter with such a definition that there will be a relation between the value of the arc identifier and the thickness of the arcs. For example the higher the transport, the thicker the corresponding arc in a transport model.



