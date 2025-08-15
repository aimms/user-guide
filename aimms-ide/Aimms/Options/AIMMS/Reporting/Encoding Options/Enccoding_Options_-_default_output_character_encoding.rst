

.. _Options_Enccoding_Options_-_default_output_character_encoding:


Default output character encoding
=================================



**Type**:	Selection	

**Range**:	The predeclared set AllCharacterEncodings	

**Default**:	Utf8	



This option sets the default encoding when a text file is written, for instance using PUT statements or Write to File statements.

Possible values for this option are the elements in the predeclared set AllCharacterEncodings.



This option is ignored if:

*	A FILE is written whereby the file identifier has a specified encoding attribute.




In order to ease the exchange of files with people located in other locales, you may want to switch to UTF8; this encoding can be used globally and unambiguously.





**Learn more about** 

*	:ref:`file.encoding`
*	:any:`AllCharacterEncodings`



