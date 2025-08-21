

.. _option-AIMMS-default_input_character_encoding:


Default input character encoding
================================



:Type:	Selection	
:Range:	The predeclared set AllCharacterEncodings	
:Default:	Utf8	



This option sets the default encoding when a text file is read in.

Possible values for this option are the elements in the predeclared set AllCharacterEncodings.



This option is ignored if:

*	A FILE is read in whereby the file identifier has a specified encoding attribute.
*	The file itself has a byte order mark determining the encoding of the file.




In order to ease the exchange of files with people located in other locales, you may want to switch to UTF8; this encoding can be used globally and unambiguously.





**Learn more about** 

*	:ref:`file.encoding`
*	:any:`AllCharacterEncodings`


