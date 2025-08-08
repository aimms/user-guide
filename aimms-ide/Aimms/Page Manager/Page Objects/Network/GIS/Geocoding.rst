

.. _Network_Geocoding:


Geocoding
=========

The intrinsic AIMMS function GeoFindCoordinates is able to find the latitude/longitude coordinates for a given address. The procedure uses the free `OpenStreetMap <https://www.openstreetmap.org>`_ (OSM) geocoding service. You are advised to carefully read the OSM geocoder `usage policy <https://wiki.openstreetmap.org/wiki/Nominatim#Usage_Policy>`_ before using this procedure in your application.



The function returns 0 when the address cannot be found. Examples of valid function calls are



  GeoFindCoordinates( "NL", Latitude, Longitude, "me@company.com" );

  GeoFindCoordinates( "Haarlem, NL", Latitude, Longitude );

  GeoFindCoordinates( "2034 Haarlem, NL", Latitude, Longitude );

  GeoFindCoordinates( "Schipholweg, Haarlem, NL", Latitude, Longitude );

  GeoFindCoordinates( "1 Schipholweg, Haarlem, NL", Latitude, Longitude );

  GeoFindCoordinates( "1 Schipholweg, 2034 Haarlem, NL", Latitude, Longitude );

  



  GeoFindCoordinates( "US", Latitude, Longitude );

  GeoFindCoordinates( "Kirkland, WA, US", Latitude, Longitude );

  GeoFindCoordinates( "Lake Washington Boulevard NE, Kirkland, US", Latitude, Longitude );

  GeoFindCoordinates( "5400 Carillon Point, Lake Washington Boulevard NE, Kirkland, US", Latitude, Longitude );

  

  GeoFindCoordinates( "Singapore", Latitude, Longitude );

  GeoFindCoordinates( "Chulia Street, Singapore", Latitude, Longitude );



assumed that ``Latitude``  and ``Longitude``  are declared as numerical parameters in your model.



**Learn more about** 



*	:any:`GeoFindCoordinates`
