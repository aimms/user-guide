

.. _Miscellaneous_Command_Line_Options_-_User:


User
====



:Long Name:	--user	
:Short Name:	-U	
:Argument	User[:password]	

When an AIMMS project is linked to an end-user database, you must logon to the project before being able to run it. Through the --user commandline option, you can specify a user name and optionally a password with which you want to logon to the system. If you specify a user name only, the logon screen will be partially filled in with the user name provided on the commandline. If you specify a password as well, AIMMS will verify its correctness and skip the logon screen altogether if the combination is accepted. Providing a user name and password is not advised for interactive use, but may be convenient when you want the model to run unattended.	



**Learn more about** 

*	:ref:`Security_User_Management`  



