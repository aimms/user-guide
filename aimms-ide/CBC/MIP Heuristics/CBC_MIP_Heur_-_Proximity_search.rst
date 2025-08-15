.. _CBC_MIP_Heur_-_Proximity_search:


Proximity search
================



**Type**:	Selection	

**Range**:	The settings listed below	

**Default**:	Off	



This option controls the use of the ”No-Neighborhood Search” 0-1 MIP reﬁnement heuristic proposed by Fischetti and Monaci (2012). The idea is to deﬁne a sub-MIP without additional constraints but with a modiﬁed objective function intended to attract the search in the proximity of the incumbent. The approach works well for 0-1 MIPs whose solution landscape is not too irregular (meaning the there is reasonable probability of ﬁnding an improved solution by ﬂipping a small number of binary variables), in particular when it is applied to the ﬁrst heuristic solutions found at the root node.



Possible values are:



*	Off
*	On



