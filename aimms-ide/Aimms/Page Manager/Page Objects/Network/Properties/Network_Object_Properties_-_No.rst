

.. _Network_Network_Object_Properties_-_No:


Nodes
=====

**Description** 

In the nodes tab of the network property dialog box, various fields concerning nodes can be set.



**Node** 

In the node field, the node in the network object whose properties are displayed is selected. If your network contains multiple node sets, then you should select the node that you want to modify here.



**Size** 

The size determines the width and height of an individual node. This can be a value, a scalar identifier or a 1-dimensional identifier, indexed over the node set. In this last case you can assign a size for each individual node. 



**Size of 1.0 equal to** 

Here you specify how the size of a node is translated into pixels on the screen. There are two options:

*	Direct translation to pixels, which is independent of the current scale of the visible area.
*	Translated to coordinate points. This means that a size of 1 is measured as an interval of 1 along the current X-axis. For example, if the left side of the visible area is currently equal to 0 and the right side equal to 10, then a size of 1 is displayed as 1/10th of the total object width. In this mode the size of the nodes will thus change if you zoom in or out.




**Size Limit** 


In this property field limits on the sizes can be specified. These limits are defined in pixels. A minimum and maximum size is specified, and nodes are never displayed smaller than the minimum size, and never larger than the maximum size.





**Shape** 


A node can be displayed either as a filled rectangle, a filled circle or a rectangle containing a bitmap. The bitmap filename should be entered as "quoted text", a scalar string parameter or a 1-dimensional string parameter, which allows different bitmaps for different elements.


If you choose a bitmap for a node, then this bitmap is shrunken / stretched to fit into a square shape.





**Selectable** 


With this property you can specify whether the user can select a node by clicking on it. 


By default a Node is selectable. If you don't want a Node to be selectable you can speficy a value equal to 0. This value can be a fixed value or an identifier, optionally indexed over the node set. 







