.. _GUROBI_General_-_Solution_File:


Solution File
=============



**Type** :	Selection	

**Range** :	The settings listed below	

**Default** :	Never	



This option can be used to activate the generation of Gurobi solution files containing the solution found. Note that this solution does not have to match with the one reported by AIMMS due to the fact that AIMMS takes care of scaling for instance. The data is written to a file called gurddddd.sol, where ddddd denotes a 5-digit sequence number. Possible values are:



*	Never
*	At the first solve
*	At every solve






