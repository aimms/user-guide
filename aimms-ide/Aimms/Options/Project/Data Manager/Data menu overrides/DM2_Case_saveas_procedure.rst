

.. _option-AIMMS-case_saveas_procedure:


Case Saveas Procedure
=====================

:Type:	Name of a procedure	
:Default:	\-	



With this option you can override the menu command **Data - Save Case As** 

If this option is not specified, AIMMS uses built-in code that does the following:


*   Let the user select the case file to save the data to,
*   Save current data to the selected case file
*   Assign the 'active case' to the selected case
*   Make current data 'clean'



Overriding this menu allows you to implement your own data management, or fine-tune the built-in data management.



