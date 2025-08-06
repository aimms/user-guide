

.. _Options_DM2_Case_save_procedure:


Case save procedure
===================

Type:	Name of a procedure	

Default:	-	



With this option you can override the menu command **Data - Save Case** 

If this option is not specified, AIMMS uses built-in code that does the following:


*   if 'active case' is not set: switch to **Data - Save Case As** 

otherwise:


*   save current data to the active case file
*   make current data 'clean'



Overriding this menu allows you to implement your own data management, or fine-tune the built-in data management.



