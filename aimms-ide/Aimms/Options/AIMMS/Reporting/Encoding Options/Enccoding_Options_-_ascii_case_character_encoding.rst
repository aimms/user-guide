

.. _Options_Enccoding_Options_-_ascii_case_character_encoding:


Ascii case character encoding
=============================



Type:	Selection	

Range:	An element of the predeclared set ASCIICharacterEncodings	

Default:	Utf8	



This option determines the encoding used to decode strings stored in a case file constructed by an ASCII AIMMS 3.13 or older release. 

Possible values for this option are the elements in the predeclared set ASCIICharacterEncodings.



If you converted your project from AIMMS 3.13 or older, the option value is set during this conversion. 



**Notes:** 

*	Cases created by AIMMS 3.14 or newer, the UTF8 encoding is used to store strings in that case, and the value of this option ignored.
*	Cases created by the Unicode AIMMS 3.13 or older, the UTF-16LE encoding is used to store strings in that case, and the value of this option ignored.




**Learn more about** 

*	:ref:`file.encoding`
*	:any:`AllCharacterEncodings`




