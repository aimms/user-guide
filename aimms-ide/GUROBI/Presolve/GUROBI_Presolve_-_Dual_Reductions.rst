.. _GUROBI_Presolve_-_Dual_Reductions:


Dual Reductions
===============



**Type** :	Selection	

**Range** :	The settings listed below	

**Default** :	Yes	



This option determines whether dual reductions are performed. Possible values are:



*	No
*	Yes




**Note** 

*	If the model uses lazy constraints (either through a callback or a pool) then Gurobi turns off dual reductions.
