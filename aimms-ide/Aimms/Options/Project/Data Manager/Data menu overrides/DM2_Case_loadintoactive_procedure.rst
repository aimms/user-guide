

.. _option-AIMMS-case_loadintoactive_procedure:


Case Loadintoactive Procedure
=============================

:Type:	Name of a procedure	
:Default:	\-	



With this option you can override the menu command **Data - Load Case - Into Active** 

If this option is not specified, AIMMS uses built-in code that does the following:


*   Let the user select a case file
*   Load the data from the selected case file into the current data (any identifier stored in the case file will completely replace the current data of that identifier)
*   The active case reference remains unchanged



Overriding this menu allows you to implement your own data management, or fine-tune the built-in data management.



