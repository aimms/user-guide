

.. _option-AIMMS-startup_page:


Startup Page
============



:Type:	Name of a page	
:Default:	\-	



This option specifies the page that is opened when starting the project.



If you also specify a startup case and/or a startup procedure, then you should know that AIMMS uses the following sequence when starting a project:

    1.	Compilation and running of MainInitialization

    2.	Load the startup case (if specified)

    3.	Run the startup procedure (if specified)

    4.	Open the startup page.



If there is no startup page, case or procedure, AIMMS will at startup only present the model editor tree and not compile the model.



**Tips & Tricks** 

*	If the sequence above is not applicable for your application, you can write a startup procedure that includes the loading of a case and the opening of a page.
*	If you want to skip the entire startup sequence while opening a project, you should hold down the Shift key during startup, until the project is opened.




**Note** 

*	The user can always go back to the start up page by clicking the First Page button on the toolbar.




**Learn more about** 

*	:ref:`Page-Manager_Page_Introduction`  



