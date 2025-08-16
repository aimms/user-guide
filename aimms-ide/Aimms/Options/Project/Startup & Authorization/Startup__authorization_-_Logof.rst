

.. _Options_Startup__authorization_-_Logof:


Logoff Procedure
================



:Type:	Name of a procedure	
:Default:	\-	



This option specifies the procedure that is executed when a user logs off from a multi-user application. This typically happens when the group, user or authorization level is changed, or a project that is linked to a user database file is closed. The logoff procedure should return a non-zero value to let the logoff process proceed. If it returns 0, then the current user remains logged on.



**Note** 

*	When changing the group, user or authorization level, running the logon procedure follows running the logoff procedure.
*	When the project is closed, first the logoff procedure is called and if this procedure returns a non-zero value, then the MainTermination procedure is called. If either of the two returns 0 the project will not be closed.




**Tips & Tricks** 

*	If each user has its own data to work with, then the logoff procedure is a good place to check whether or not the user should save its data. You can do this by copying the default contents of the procedure MainTermination to the body of the logoff procedure (and let MainTermination simply return 1).




**How to ...** 

*	:ref:`Security_Linking_to_a_User_Database`  
*	:ref:`Options_Startup__authorization_-_Logon`  
*	:ref:`Security_Changing_Group_within_an_Appli`  
*	:ref:`Security_Changing_User_within_an_Applic`  
*	:ref:`Security_Changing_Authorization_Level_w`  




**Learn more about** 

*	:ref:`Model-Explorer_Procedures`  
*	:ref:`Security_User_Management`  
*	:ref:`Options_Startup__authorization_-_Logon`  



