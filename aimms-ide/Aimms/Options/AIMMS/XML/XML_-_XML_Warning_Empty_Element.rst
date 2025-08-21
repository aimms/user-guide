.. _option-AIMMS-xml_warning_empty_element:

XML Warning Empty Element
=========================

:Type:   Selection   
:Range:  The settings listed below   
:Default:    On  

By default, when reading an XML file, AIMMS checks for empty elements that are assigned to a set. If the XML reader finds such an empty set element then AIMMS will generate a warning. AIMMS will not generate warnings if you switch off this option. Possible values are:

*   Off
*   On

**Example** 

Consider the following XML mapping file:

.. code-block:: xml

    <AimmsXMLSchemaMapping xmlns="https://www.aimms.com/XMLSchema/AimmsXMLMappingSchema">
      <ElementMapping name="City1">
        <AttributeMapping name="elem" binds-to="i"/>
        <ElementMapping name="City2">
          <AttributeMapping name="elem" binds-to="j"/>
          <AttributeMapping name="dist" maps-to="Distance(i,j)"/>
          <AttributeMapping name="dmd" maps-to="Demand(i)"/>
        </ElementMapping>
      </ElementMapping>
    </AimmsXMLSchemaMapping>

Assume we have the following data snippet in the XML data file:

.. code-block:: xml

    <City1 elem="Amsterdam">
       <City2 dist="145" dmd="30"/>
    </City1>

AIMMS will not assign any data to the parameter Distance because no element is assigned to "j". 
Moreover, AIMMS will also not assign data to the parameter Demand (although it does not depend on "j") because 
all data corresponding to identifiers below "j" in the mapping file will be ignored. 
If this option is switched on then AIMMS will generate a warning.

