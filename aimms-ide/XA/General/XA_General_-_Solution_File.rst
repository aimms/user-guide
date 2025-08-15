.. _XA_General_-_Solution_File:


Solution File
=============



**Type**:	Selection	

**Range**:	The settings listed below	

**Default**:	Never	



This option can be used to activate the generation of XA solution files containing the found solution. Note that this solution does not necessarily have to match with the one reported by AIMMS. For example, this can be due to the fact that AIMMS takes care of scaling as well. The data is written to a file called axddddd.sol, where ddddd denotes a 5 digits sequence number. Possible values are:



*	Never
*	At the first solve
*	At every solve



