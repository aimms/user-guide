.. |img_def_GIS_Warning_Symbol_gif| image:: images/GIS_Warning_Symbol.gif


.. _Network_UsingGISinAIMMS:


Using GIS in AIMMS
==================

The new GIS features in AIMMS are available as part of the existing page network object. A GIS map can be displayed as the background image of a network. When you decide not to specify any node and arcs for the network object, the network object will serve as a map viewer object that still provides zoom and scroll functionality.



When specifying a GIS map as the background for your network object, please keep in mind that the visible area of the network should be within the rectangle (left=-180, bottom=-90, right=180, top=90) which corresponds to the GIS coordinates of the world. AIMMS automatically adjusts the rectangle by removing any parts outside the maximum rectangle.



To specify a GIS map in AIMMS you need to specify


*   an unordered list of GIS sources (e.g. a GIS server, a local file), and
*   an ordered list of layers. Every layer should be associated to exactly one source. The actual map image is obtained by overlaying the individual layer images in the specified order.



When an error occurs during communication with a GIS server (e.g. connection error, timeout error, invalid layer name), the error is reported as a warning to the AIMMS message window. In developer mode the network object will display a small warning icon |img_def_GIS_Warning_Symbol_gif| in its upper left corner to indicate that the GIS communication generated some errors. In this case you are advised to inspect the message window. In developer as well as in end-user mode, the displayed GIS information is restricted to the parts that were retrieved successfully.



