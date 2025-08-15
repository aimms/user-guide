.. _ODH-CPLEX_XGeneral_-_Ord_File:


Ord File
========



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Never	



When this option is switched on, an ORD file is generated containing the priority orders of the variables in the model. The data will be written to a file called cpxddddd.ord, where ddddd denotes a 5-digit sequence number. Possible values are:



*	Never
*	At the first solve
*	At every solve




In AIMMS and CPLEX variables with highest priorities are given preference over variables with lowest priorities.




