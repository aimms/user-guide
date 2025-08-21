

.. _option-AIMMS-solution_batch_size:


Solution Batch Size
===================



:Type:	Integer	
:Range:	{10..10000000}	
:Default:	1000000	



This option limits the size of the batches that are used to retrieve the solution from the solver. A large batch size will usually be more efficient but requires more memory. The actual batch size used is limited by the number of columns and rows in the generated math program.

