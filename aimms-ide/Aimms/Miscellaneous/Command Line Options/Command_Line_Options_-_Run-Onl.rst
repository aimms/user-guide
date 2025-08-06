

.. _Miscellaneous_Command_Line_Options_-_Run-Onl:


Run-Only
========



Long Name:	--run-only	

Short Name:	-R	

Argument:	Procedure name	

Description:	When you want to run an AIMMS project unattended, you can call AIMMS with the --run-only option. This option expects the name of a procedure in the model, which will be executed after the project is opened. After running the procedure, the AIMMS session will be terminated. You can only specify the --run-only option if you also specify a project file on the commandline. Note that actions upon open project, such as load a case, open a page, execute a procedure, are not performed in run-only mode. MainTermination is executed.	





