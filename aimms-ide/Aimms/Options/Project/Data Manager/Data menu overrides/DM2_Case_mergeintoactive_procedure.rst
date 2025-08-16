

.. _Options_DM2_Case_mergeintoactive_procedure:


Case mergeintoactive procedure
==============================

:Type:	Name of a procedure	
:Default:	\-	



With this option you can override the menu command **Data - Load Case - Merging Into Active** 

If this option is not specified, AIMMS uses built-in code that does the following:


*   let the user select a case file
*   merge the data from the selected case file with the current data (the current data will only be overwritten by the non defaults stored in the case file)
*   the active case reference remains unchanged



Overriding this menu allows you to implement your own data management, or fine-tune the built-in data management.



