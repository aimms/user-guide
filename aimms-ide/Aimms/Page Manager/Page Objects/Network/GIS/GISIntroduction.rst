

.. _Network_GISIntroduction:


Introduction
============

**Open Geospatial Consortium** 

AIMMS supports the display of GIS data, i.e. data provided by Geographical Information Systems.



**Sources** 

AIMMS supports several types of map sources:


*    OGC Web Map Service ``https://www.ogc.org/standards/wms/``
*    `Yahoo! Maps <https://search.yahoo.com/>`_
*    `Bing Maps <https://www.bing.com/maps/>`_
*    `OpenStreetMap <https://www.openstreetmap.org/>`_
*    locally stored `ESRI <https://www.esri.com/en-us/home>`_ shape files, the format as used by ArcGIS and ArcView,
*    locally stored feature data stored in OGC `Geography Markup Language ``https://www.ogc.org/standards/gml`` (GML) format, 
*    locally stored map image files



**Disclaimer** 

All usage of map data is subjective to license terms set forth by the holders of this map data (Yahoo!, Bing, OpenStreetMap, etc.). 
The use of these sources in any of our examples is meant for illustrative purposes only and does not imply any usage rights for AIMMS license holders. 
It is the user's responsibility to be compliant with the licenses agreement of the respective providers when using map data sources.



**Web Map Service** 

One of the OGC standards considers connections to a Web Map Service (WMS). 
To obtain map data from a WMS server AIMMS sends a HTTP request to a WMS server. 
This request contains the map parameters that the server needs to render the map build up from a collection of layers (see below). 
The rendered map is then sent back to AIMMS.



**Web Feature Service** 

A second OGC standard that AIMMS supports is the connection to a Web Feature Service (WFS). 
Feature data consists of data related to geographical structures (e.g. point, lines, polygons). 
The requested feature data is sent back to AIMMS in the form of an GML document (see below). 
This GML document is parsed by AIMMS. The parsed feature data is then rendered upon the map image.



Note that many freely available WMS and WFS servers exist. 
However, it is outside the scope of this manual to detail and list them.



**Yahoo! Maps** 

Besides the OGC standards AIMMS is able to use maps provided by Yahoo! Maps. 
Yahoo! Maps automatically shows more detail as the zoom level increases and are very suitable for displaying road maps on state, 
city or street level. Note that Yahoo! Maps uses a :ref:`Network_MapProjections`  and 
should therefore not be combined with sources that do not support Mercator projections nor superimposed with arcs and nodes!



**Bing Maps** 

In addition, AIMMS is also able to retrieve map data from Microsoft Bing Maps. Similar to Yahoo! Maps and OpenStreetMap data, 
the maps from Bing Maps show more detail as the zoom level increases and they use a :ref:`Network_MapProjections` .



**OpenStreetMaps** 

OpenStreetMap (OSM) provides data similar to Yahoo! and Bing Maps with the difference that the OSM data 
can be freely used in your application as long as you comply with the OSM `license <https://www.openstreetmap.org/copyright>`_. 
Similar to Yahoo! and Bing Maps, OSM uses a :ref:`Network_MapProjections` .



**Local ESRI Shape Files** 

The ESRI Shape File is a geospatial data format developed and regulated by ESRI. 
Shape files commonly refer to a collection of files with ".shp", ".shx", ".dbf", and 
other extensions on a common prefix name (i.e., "schools.*"). 
The actual Shape File relates specifically to files with the ".shp" extension, 
however this file alone is incomplete for distribution, as it depends on the other supporting files. 
Shape Files spatially describe points, polygons, polylines.


**Local GML Files** 

Besides connections to the above GIS standards, AIMMS also supports the import of local GML data. 
The GML format is a special XML format that is designed by the OGC to support the description and 
communication of geographic feature data. The GML document is parsed by AIMMS and 
the parsed feature data is then rendered upon the map image.

The simple and freely available command line utility `ogr2ogr <https://gdal.org/en/stable/programs/ogr2ogr.html>`_ 
is able to convert between ESRI Shape and GML format.



**Local Image Files** 

To complement the local storage data (in ESRI Shape or GML format), AIMMS also supports the use of local map image files. 
In applications were no internet connection is available, a local image file combined with several ESRI Shape or GML layers 
can still be used to construct a useful background map for the network object in which the application has control 
over some properties of the features stored in the ESRI Shape or GML format (see the 'GIS Support' example 
(in the AIMMS 'Examples' folder) for an example of how to control the color of areas based on model data). 
Obviously, no new image data is retrieved when the user zooms or scrolls the image. Instead, the zooming and scrolling will graphically zoom and/or move the image.



**Layers** 

Each of the above eight source types can provide one or more layers that together will build up the map image. 
WMS en WFS servers can provide multiple layers (each representing one kind of geographical data) 
while the other only provide a single layer. For example, a map image retrieved from a WMS server can be built up from two layers, 
'Bathymetry', a layer showing the oceans, and 'Topography', a layer showing land. On top of this a collection of GML layers can be drawn, 
each layer describing (the boundary of) a single state. Each layer is rendered upon the image in the order as specified. 
Note that GIS servers might consider to display more or less information when the image scale allows for it. For example, 
it makes no sense to display road information when the image is zoomed to the extent of the whole earth.



