

.. _Options_XML_-_XML_Encoding:


XML Encoding
============



Type:	Selection	

Range:	The settings listed below	

Default:	Automatic	



When AIMMS data is written to an XML file the characters are represented by (hexadecimal) numbers according to some encode mapping. By using the same encoding an XML parser can translate these numbers back to characters. The possible values for the encoding are:



*	Automatic
*	ISO-8859-1 (European language characters 8 bit)
*	UTF-8 (Unicode character encoding for English language characters 8 bit)
*	UTF-16 (Unicode character encoding 16 bit)







**Remark** 


Typically, 'UTF-16' is used for writing Unicode, and 'UTF-8' and 'ISO-8859-1' for writing ASCII. The default setting of the option 'XML encoding' is 'Automatic', meaning that for a ASCII version of AIMMS the encoding will be set to 'ISO-8859-1' and for a UNICODE version of AIMMS to 'UTF-16'.




