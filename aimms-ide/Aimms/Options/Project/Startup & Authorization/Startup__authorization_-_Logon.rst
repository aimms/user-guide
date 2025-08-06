

.. _Options_Startup__authorization_-_Logon:


Logon Procedure
===============



Type:	Name of a procedure	

Default:	-	



This option specifies the procedure that is executed when a user logs on to a multi-user application. This typically happens when the group, user or authorization level is changed.



**Note** 

*	The logon procedure is only applicable if the project is linked to a user database file.
*	The logon procedure is automatically called whenever you change the current user, current group or current authorization level, except during the initial logon. If the project is started, the logon dialog box will appear, but the logon procedure is not executed automatically. Because it is a priori not clear when this procedure must run (in combination with startup page, startup case, and/or startup procedure), you must manually add a call to the logon procedure in the body of the startup procedure.
*	If you also specify a logoff procedure, then, when changing the group, user or authorization level, the logoff procedure is called before the logon procedure.




**Learn more about** 

*	:ref:`Model-Explorer_Procedures`  
*	:ref:`Options_Startup__authorization_-_Logof`  
*	:ref:`Options_Startup__authorization_-_star2`  
*	:ref:`Security_User_Management`  



