

.. _Options_DM2_Case_saveas_procedure:


Case saveas procedure
=====================

Type:	Name of a procedure	

Default:	-	



With this option you can override the menu command **Data - Save Case As** 

If this option is not specified, AIMMS uses built-in code that does the following:


*   let the user select the case file to save the data to,
*   save current data to the selected case file


*   assign the 'active case' to the selected case


*   make current data 'clean'



Overriding this menu allows you to implement your own data management, or fine-tune the built-in data management.



