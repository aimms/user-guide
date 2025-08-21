.. _option-GUROBI-hints_file:


Hints File
==========



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Off	



This option determines whether a hints file should be read or written by Gurobi. Possible values are:



*	Off
*	Read
*	Write




If this option is set to 'Read' then the hints file will be read. The hints file should be named 'gurobi.hnt' and be placed in the AIMMS project directory (which is the directory that contains the .aimms file). If this option is set to 'Read' then hints information in the AIMMS project will be ignored.





If this option is set to 'Write' then a hints file will be written. The hints file will be named 'gurobi.hnt' will be written in the AIMMS project directory.

