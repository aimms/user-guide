

.. _option-AIMMS-case_string_character_set:


Case String Character Set
=========================



:Type:	Selection	
:Default:	Native



A case file may contain many strings, both for the values of string parameters and for the element names. Reading
and writing these strings may be time expensive and besides that the strings have an effect on big the case file is.	

If your cases are saved and loaded only on the same platform (either Windows or Linux) then it might be favorable
to just store these strings using the 'native' unicode character encoding (which is UTF16LE on windows, and UTF32LE on linux). 

Especially on Linux converting all the strings from a non-native encoding may have a negative impact on the total
time that is needed to write or read a case. In other words, if your case files are shared between operating systems,
it might be favorable always store the strings using Native_Linux. This is certainly the fastest on Linux, and on
Windows the effect of needing to convert is not really bad.

Possible values are:

    *	UTF8 (produces the smallest cases)
    *	Native (for the current operating system, translates to either Native_Linux or Native_Windows)
    *	Native_Linux (requires the option **Case Compatibility** to be at set to 'Aimms 4 80')
    *	Native_Windows (requires the option **Case Compatibility** to be at set to 'Aimms 4 80')


**Learn more about** 

*	:ref:`option-AIMMS-case_compatibility`  

