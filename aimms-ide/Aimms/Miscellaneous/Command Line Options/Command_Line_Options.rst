.. _Miscellaneous_Command_Line_Options:

Command Line Options
====================

**Description** 

On the AIMMS commandline, you can specify a number of options and arguments that will influence the manner in which AIMMS is started. 
The following line illustrates the general structure of a call to the AIMMS executable.

AIMMS [commandline-options] [project-file [session-arguments]]

All options start with a minus sign and some require a single argument. 
For a number of commandline options AIMMS offers both long and short option names. 
While the long option names are easier to remember, 
the short option names allow for a more compact commandline. 
Short option names without an argument may be appended after a single minus sign.

AIMMS will interpret the first non-option argument on the commandline as the name of the project file 
with which you want to open AIMMS. 
If you specify a project file, the settings of the project may initiate model-related execution or 
automatically open a page within the project. 
If you want to open a project for editing only, and do not want these initial actions to take place, 
you should hold down the Shift key when opening the project. 
The initial actions are also not performed when the commandline also contains the --run-only option, 
in which case all execution must take place from within the specified procedure.

Directly after the name of the project file, AIMMS allows you to specify an arbitrary number of string arguments,
which are not interpreted by AIMMS, but can be used to pass commandline information to the project. 
In the model, you can obtain the values of these string arguments one at a time through 
the predefined function :any:`SessionArgument`, which is explained in more detail in the Language Reference.

**Learn more about the commandline-options** 

*   :ref:`Miscellaneous_Command_Line_Options_-_User`  
*   :ref:`Miscellaneous_Command_Line_Options_-_Backup-`  
*   :ref:`Miscellaneous_Command_Line_Options_-_Log-Dir`  
*   :ref:`Miscellaneous_Command_Line_Options_-_Config-`  
*   :ref:`Miscellaneous_License`  
*   :ref:`Miscellaneous_Command_Line_Options_-_Run-Onl`  
*   :ref:`Miscellaneous_Command_Line_Options_-_Minimiz`  
*   :ref:`Miscellaneous_Command_Line_Options_-_Maximiz`  
*   :ref:`Miscellaneous_Command_Line_Options_-_Hidden`  
*   :ref:`Miscellaneous_Command_Line_Options_-_As_Serv`  
*   :ref:`Miscellaneous_Command_Line_Options_-_End-Use`  
*   :ref:`Miscellaneous_Command_Line_Options_-_Help`  
*   :ref:`Miscellaneous_Command_Line_Options_-_User-da`  


**Learn more about** 

*    :any:`SessionArgument` 



