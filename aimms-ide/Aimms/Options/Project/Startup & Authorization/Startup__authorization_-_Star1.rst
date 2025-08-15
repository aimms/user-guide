

.. _Options_Startup__authorization_-_Star1:


Startup Case
============



**Type**:	Name of a case	

**Default**:	-	



This option specifies the case that is opened automatically when starting the project.



If you also specify a startup procedure and/or a startup page, then you should know that AIMMS uses the following sequence when starting a project:

1.	Compilation and running of MainInitialization

2.	Load the startup case (if specified)

3.	Run the startup procedure (if specified)

4.	Open the startup page.



If there is no startup page, case or procedure, AIMMS will at startup only present the model editor tree and not compile the model.



**Tips & Tricks** 

*	If the sequence above is not applicable for your application, you can write a startup procedure that includes the loading of a case and the opening of a page.
*	If you want to skip the entire startup sequence while opening a project, you should hold down the Shift key during startup, until the project is opened.






