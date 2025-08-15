.. _CONOPT_Parallel_-_Thread_Limit:

Thread Limit
============



**Type**:	Integer	

**Range**:	{0..:ref:`Miscellaneous_Maxint` }	

**Default**:	1	



This option determines the default number of parallel processes (threads) that will be invoked by CONOPT. CONOPT can use multiple threads for some internal computations and for function and derivative evaluations (through AIMMS). Multiple threads are currently only used for certain fairly large and dense computations and these models are quite rare. In addition, multiple threads have a quite high overhead and they are therefore only useful for fairly large models. Currently the best improvements have been for very large models with more than 100,000 variables or constraints.



The value of 0 sets the thread count equal to the number of processors in the machine.

