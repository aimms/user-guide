

.. _option-AIMMS-number_of_execution_threads:


Number of Execution Threads
===========================



:Type:	Integer	
:Range:	{0 .. maxint}
:Default:	0	

With this option you can change how many threads, that is (virtual) processor cores, a single assignment statement or definition evaluation may use.
It only has an effect on indexed expressions, with either a large domain and/or a complex expression. Simple small or scalar expressions are always evaluated single threaded.

By default it is set to 0 which means that it will take all available cores. If you set it to a number that is higher than the number of cores on your machine it will behave as if it was not set and thus use all available cores.













