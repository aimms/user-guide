

.. _Options_DM2_Case_loadintoactive_procedure:


Case loadintoactive procedure
=============================

**Type**:	Name of a procedure	

**Default**:	-	



With this option you can override the menu command **Data - Load Case - Into Active** 

If this option is not specified, AIMMS uses built-in code that does the following:


*   let the user select a case file
*   load the data from the selected case file into the current data (any identifier stored in the case file will completely replace the current data of that identifier)
*   the active case reference remains unchanged



Overriding this menu allows you to implement your own data management, or fine-tune the built-in data management.



