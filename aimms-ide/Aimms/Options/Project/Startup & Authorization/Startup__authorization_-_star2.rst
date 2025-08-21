

.. _option-AIMMS-startup_procedure:


Startup Procedure
=================



:Type:	Name of a procedure	
:Default:	\-	



This option specifies the procedure that is executed automatically when starting the project. In the startup procedure you can setup the initial working environment for a (specific) user. For example you let the user pick a startup case, open a page, initiate a database link, etc.

If you also specify a startup case and/or a startup page, then you should know that AIMMS uses the following sequence when starting a project:

1.	Compilation and running of MainInitialization

2.	Load the startup case (if specified)

3.	Run the startup procedure (if specified)

4.	Open the startup page.



If there is no startup page, case or procedure, AIMMS will at startup only present the model editor tree and not compile the model.



**Tips & Tricks** 

*	If the sequence above is not applicable for your application, you can write a startup procedure that includes the loading of a case and the opening of a page.
*	If you want to skip the entire startup sequence while opening a project, you should hold down the Shift key during startup, until the project is opened.




**Learn more about** 

*	:ref:`Model-Explorer_Procedures`  



