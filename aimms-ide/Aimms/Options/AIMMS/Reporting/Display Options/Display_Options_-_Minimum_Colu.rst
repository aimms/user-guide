

.. _Options_Display_Options_-_Minimum_Colu:


Minimum Column Fill Percentage Tabular Display
==============================================



:Type:	Integer	
:Range:	{ 0 .. 101}	
:Default:	5	



This option determines how data of 2 or 3 dimensional identifiers should be written to file. This can be in tabular format or list format. When the filling percentage, this is 100 times the average number of elements per row divided by the maximal number of elements per row, is smaller than the value of this option, the identifiers will be written in list format, otherwise the identifiers will be written in tabular format. Please realize that setting this option to a low value and the option Listing Page Width to a large value can lead to large output files when writing sparse identifiers to file.



**Learn more about** 

*	:ref:`Options_Listing_Format_Options_-_Listi`  






