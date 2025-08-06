

.. _Miscellaneous_User_Logoff:


User Logoff
===========

**Description** 

When multiple users want to use the same application on the same computer, the first user can log off. When a user logs off, the project will not be closed, but a dialog box will appear in which you can type another user name and password. A user can log off by selecting Authorization Logoff… from the File menu.



**Note** 

*	If you have specified a Logoff procedure in the Project Options dialog box, then this logoff procedure will be run before actually logging of the user. This procedure should return a nonzero value to allow the user to logoff. If the procedure returns 0, then the user remains logged on. Usually you use the logoff procedure to inform the user of unsaved data and allow him to save this data in a case.
*	If you have specified a Logon procedure in the Project Options dialog box, then this procedure will automatically be run after a new user has logged in.



