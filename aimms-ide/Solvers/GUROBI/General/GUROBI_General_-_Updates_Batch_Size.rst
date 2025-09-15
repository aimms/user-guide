.. _option-GUROBI-updates_batch_size:


Updates Batch Size
==================



:Type:	Integer	
:Range:	{10 .. 10000000}	
:Default:	1000000	



This option limits the size of the batches that are used to pass :ref:`GMP <sec:gmp.intro>` updates to Gurobi after, e.g., modifying
matrix coefficients using GMP functionality. A large batch size will usually be more efficient but requires more memory. The actual
batch size used is limited by the number of updates.

