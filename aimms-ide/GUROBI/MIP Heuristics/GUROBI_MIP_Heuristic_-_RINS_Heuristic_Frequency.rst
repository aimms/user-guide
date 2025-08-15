.. _GUROBI_MIP_Heuristic_-_RINS_Heuristic_Frequency:


RINS Heuristic Frequency
========================



**Type**:	Integer	

**Range**:	{-1 .. 2000000000}	

**Default**:	-1	



This option set the frequency of the RINS heuristic. The default value of -1 chooses automatically. A value of 0 shuts off RINS. A positive value n applies RINS at every n-th node of the MIP search tree.

