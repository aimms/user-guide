

.. _Options_Appearance_Number_1000_Separat:


Number 1000 Separator
=====================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Comma (1,000,000)	



This option determines in which format large numbers (>1000) are displayed in pages. Possible values are:



*	Comma (1,000,000)
*	Period (1.000.000)
*	Space (1 000 000)
*	Use regional settings of Windows




When this option is set to "Use regional settings of Windows", then the format of numbers is determined depending on the "Digit grouping symbol" setting, which is a setting that can be found in the "Number" tag of the "Regional settings" of the "Windows Control Panel".





**Note** 

*	If the Windows settings are used and the "Digital grouping symbol" is valued ".", then the number "1.2" is an invalid value.
*	Only the format of numbers on pages is influenced by this option and the numbers formatted using the function FormatString with %tn, %ti, and %tf in the format string.



