.. _Security_Changing_User_within_an_Applic:

Changing User within an Application
===================================

**Description** 

If you temporary want to change to another user, for example for maintenance or demonstration purposes, you can change the current user. 
Changing the current user will only change the value of the AIMMS identifier ``CurrentUser`` . 
The values of the AIMMS identifiers ``CurrentGroup``  and ``CurrentAuthorizationLevel``  will not change (for that, you should logoff and re-logon).



To change the current user:

1.	From the File menu, open the Authorization submenu and select the User command,

2.	From the drop down list, select the new user,

3.	In the password field, enter the corresponding password,

4.	Press Ok (or press Cancel to abort the operation)



**Learn more about** 

*	:any:`CurrentUser`
*	:any:`CurrentGroup`
*	:any:`CurrentAuthorizationLevel`



