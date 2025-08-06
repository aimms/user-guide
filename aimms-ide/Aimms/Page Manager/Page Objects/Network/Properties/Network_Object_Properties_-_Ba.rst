

.. _Network_Network_Object_Properties_-_Ba:


Background
==========

**Description** 

In the Background tab of the network property dialog box you can specify the background picture on top of which the arcs and nodes are drawn. This picture can be provided by an image file or it can be obtained from a GIS source.



**Background** 

To specify the background for your network object you can choose from 'No Image', an image 'From File' or an image 'From GIS Source'. 



**From File** 

Several image file format are supported (e.g. BMP, ICON, GIF, JPEG, Exif, PNG, TIFF, WMF, and EMF).



**Image File Name** 

In this field you can specify the bitmap you want to show as the background of the network object. This can be a image file name, an image from the project file, or a string parameter specifying an image file.



**Left, Right, Top & Bottom** 

By specifying the proper values for these four properties of the image file, you can synchronize the position of the image with the coordinates of the network object.



**From GIS Source** 

When specifying a GIS map as the background for your network object, please keep in mind that the visible area of the network should be within the rectangle (left=-180, bottom=-90, right=180, top=90) which corresponds to the GIS coordinates of the world. AIMMS automatically adjusts the rectangle by removing any parts outside the maximum rectangle.



To specify a GIS map in AIMMS you need to specify


*   an unordered list of GIS sources (e.g. a GIS server, a local file), and
*   an ordered list of layers

Every layer should be associated to exactly one source. The GIS map image is obtained by rendering the individual layer images in the specified order.



**Coordinate Reference System** 

A string property indicating the coordinate reference system as described :ref:`Network_MapProjections` . The default value for this property is "EPSG:4326".



**Autocorrect Lateral Distortion** 

A binary option to indicate whether AIMMS should autocorrect lateral distortion. By default this option is set to true while it provides more common images in combination with the default coordinate reference system.



For each source the following properties are available.



**Name** 

A string property used to uniquely identify (and reference) the source, not used to retrieve GIS data. When an indexed string parameter is used to specify this property, it is also possible to specify the other source properties in terms of the domain of the indexed identifier. This way a number of similar sources can be created in a generic manner. Note that duplicate source names should not be used, also taking into account the values of string parameters used.



**Type** 

A string indicating the type of the source. Currently the following source types are available 


*   WMS, which produces a map image, built up from a selection of layers,
*   WFS, which produces geographic feature data, built up from a selection of layers,
*   GML, which produces geographic feature data,
*   ESRI, which produces geographic feature data,
*   Yahoo! Map, which produces a map image,
*   Bing Maps, which produces a map image,
*   OpenStreetMap, which produces a map image, and
*   File, which obviously produces a map image.



A more detailed description of each source type can be found :ref:`Network_GISIntroduction` . Below the properties will be listed for each of the above types



**WMS and WFS Source Properties** 



**URL** 

A string property that is used to specify the URL of the server. 



Note that many freely available WMS and WFS servers exist; but it is outside the scope of this manual to list / detail them.



**Version** 

A string indicating the version of the server. The default version for "WMS" servers is "1.1.1" and the default version for "WFS" servers is set to "1.1.0"



**Proxy, Username & Password** 

String properties to specify the address of an optional proxy server, and/or an optional username and password needed to access the server



**GML Source Properties** 



**GML File** 

A filename property that refers to the GML file that contains the geographical data.



**Parsmode** 

A string property indicating whether or not the GML file should be parsed according to some standard. The default value for this property is "No validation" (which is also the quickest), but you can also choose "GML2" or "GML3" to parse the contents of the GML file according to the GML2 or GML3 standard.



**ESRI Source Properties** 



**Shape File** 

A filename property that refers to the ``*.shp``  shape file that contains part of the geographical data. Note that the corresponding ``*.dbf``  and ``*.shx``  file should also be located at the same location as the ``*.shp``  shape file.



Detailed geographical maps are available as ESRI Shape Files from several commercial sources. 
For example, `GfK GeoMarketing <https://nielseniq.com/global/de/products/geomarketing/>`_ 
offers detailed zip code/postcode area maps for a large number of countries in the world. 



**Yahoo! Map Source Properties** 



No specific Yahoo! Map source properties are available.



**Bing Maps Source Properties** 



No specific Bing Maps source properties are available.



**OpenStreetMap Source Properties** 



**URL** 

A optional string property that is used to specify the URL of an alternative OSM server (the OSM server software and data are even available for you to run on your own server). If not specified, the default OSM at ``http://tile.openstreetmap.org/``  is being used. 



**File Source Properties** 



**Image File** 

A filename property that refers to the file that contains the map image.



**Left, Right, Top & Bottom** 

By specifying the proper values for these four properties of the image file, you can synchronize the position of the image with the coordinates of the other layers and nodes in the network object.



**Layer Properties** 



**Name** 

A string property used to uniquely identify the layer, not used to retrieve GIS data. Again, an indexed string parameter may be specified here. Indexed layers can be useful to specify a set of layers all corresponding to the same source, or to specify a set of layers each corresponding to a distinct source. Note that duplicate layer names should not be used, also taking into account the values of string parameters used.



**Source** 

A string reference to a name of one of the sources in the source list that should provide the specified layer.



**External Name** 

A string indicating the name of the layer as it is known at the source. This property is only available for layers that are to be retrieved from "WMS" and "WFS" servers.



**Show Layer** 

A numerical parameter indicating whether or not the layer should be visible. The AIMMS GUI developer could use this option to give his end users some kind of control about the layers displayed in the map.



"WFS", "GML" and "ESRI" layers contain geographic feature data that is rendered on the local machine. During this rendering process some properties are available to influence the appearance of the rendered image.



**Fill Color** 

A color or color parameter to indicate the color to be used to fill closed polygons.



**Line Color** 

A color or color parameter to indicate the line color used during rendering.



**Line Width** 

A numerical parameter to indicate the width of the lines during rendering. The default line width is set to 1.



**Point Size** 

A numerical parameter to indicate the size of points during rendering. The default point size is set to 10.



**Point Style** 

A string indicating the shape to be drawn for each point to be rendered. Available style are "Triangle", "Square", "Circle", "Star", "Diamond", "Cross", "Arrow", "Pushpin", "X", "Exclamation", "Dollar", "Male", "Female", "Car", "Airplane", "Bus", "Train", "Highway", "House", and "Building". The default point style is set to "Circle".



**Learn more about** 

*	:ref:`Miscellaneous_User_Files_in_the_Project_File`  



