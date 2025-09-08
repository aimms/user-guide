

.. _option-AIMMS-case_loadasactive_procedure:


Case Loadasactive Procedure
===========================

:Type:	Name of a procedure	
:Default:	\-	



With this option you can override the menu command **Data - Load Case - As Active** 

If this option is not specified, AIMMS uses built-in code that does the following:


*   Check whether current data is 'clean' or needs to be saved first
*   Let the user select a case file
*   Load the data from the selected case file
*   Assign the 'active case' to the selected case
*   Make current data 'clean' 



Overriding this menu allows you to implement your own data management, or fine-tune the built-in data management.



