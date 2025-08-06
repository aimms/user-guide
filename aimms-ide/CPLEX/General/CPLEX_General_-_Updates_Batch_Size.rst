.. _CPLEX_General_-_Updates_Batch_Size:


Updates Batch Size
==================



**Type** :	Integer	

**Range** :	{10 .. 10000000}	

**Default** :	1000000	



This option limits the size of the batches that are used to pass model updates to CPLEX after, e.g., modifying matrix coefficients using GMP functionality. A large batch size will usually be more efficient but requires more memory. The actual batch size used is limited by the number of updates.

