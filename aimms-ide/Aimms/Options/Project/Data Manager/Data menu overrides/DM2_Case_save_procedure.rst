

.. _option-AIMMS-case_save_procedure:


Case Save Procedure
===================

:Type:	Name of a procedure	
:Default:	\-	



With this option you can override the menu command **Data - Save Case** 

If this option is not specified, AIMMS uses built-in code that does the following:


*   If 'active case' is not set: switch to **Data - Save Case As** 

otherwise:


*   Save current data to the active case file
*   Make current data 'clean'



Overriding this menu allows you to implement your own data management, or fine-tune the built-in data management.



