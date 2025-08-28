.. _option-ODHCPLEX-updates_batch_size:


Updates Batch Size
==================



:Type:	Integer	
:Range:	{10 .. 10000000}	
:Default:	1000000	



This option specifies the size of the batches that are used to pass matrix updates to CPLEX after, e.g., modifying the matrix coefficients using GMP functionality. A large batch size will usually be more efficient but require more memory. The actual batch size used is limited by the total number of matrix updates.

