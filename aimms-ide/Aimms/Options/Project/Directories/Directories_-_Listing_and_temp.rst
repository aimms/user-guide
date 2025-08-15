

.. _Options_Directories_-_Listing_and_temp:


Listing and Temporary Files
===========================



**Type**:	Name of a directory	

**Default**:	Log	



This option specifies the directory in which AIMMS writes listing and temporary files.



The specified folder name is relative to the project folder (i.e. the folder in which the .aimms file is located). In end-user situations this folder may not be writable, so then you must specify some other folder location.

To help you in specifying a valid writable location for this folder, you can use names of environment variables in this specification.

For example:



``%APPDATA%\MyProject\MyLogFiles`` 



The system will expand the string %APPDATA% with the current value of the environment variable APPDATA.



To see a list of environment variables and their current values, get a command prompt (Run: Cmd) and type the command: SET

Some interesting variables in this list are: APPDATA, USERPROFILE, USERNAME. These usually exist in any windows installation and are dependent on the currently logged on user.



