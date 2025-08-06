

.. _Options_Startup__authorization_-_Post_compile:


Post Compilation Procedure
==========================



Type:	Name of a procedure	

Default:	-	



This option specifies a procedure that is executed each time that a developer does an explicit compilation. In other words: if you select the command Run-Compile All (F5) from the menu, and the compilation was successful this procedure will be run.

This is a developer only option, as in an end-user system the Compile All command cannot be selected.





**Tips & Tricks** 


*   If you still want to have a choice whether this procedure is run after each F5 you can start the procedure with a call to DialogAsk("Do you want to run this", "Yes", "No").
*   One of the use cases for this option is the running of a set of tests each time a developer has made a change to the model. 





