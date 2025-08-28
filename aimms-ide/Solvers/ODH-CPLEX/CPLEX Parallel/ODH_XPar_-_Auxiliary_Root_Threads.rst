.. _option-ODHCPLEX-auxiliary_root_threads:


Auxiliary Root Threads
======================



:Type:	Integer	
:Range:	{-1 .. 2100000000}	
:Default:	0	



This option partitions the the number of threads for CPLEX to use for auxiliary tasks while it solves the root node of a problem. An example of an auxiliary task at the root node is the usage of root node heuristics.



On a system that offers N global threads, if you set this option to n, where



	N > n > 0



then CPLEX uses at most n threads for auxiliary tasks and at most N-n threads to solve the root node. The number of global threads is determined by the option **Global Thread Limit** . 



Independent of this option, CPLEX will never use more threads than those defined by the **Global Thread Limit**  option. CPLEX also makes sure that there is at least one thread available for the main root tasks. For example, if you set the global threads option to 3 and the auxiliary root threads option to 4, CPLEX still uses only two threads for auxiliary root tasks in order to keep one thread available for the main root tasks.



At its default value, 0, CPLEX automatically chooses the number of threads to use for the primary root tasks and for auxiliary tasks. At the value of -1, CPLEX does not use extra threads for auxiliary tasks.



**Note** 

*	The value of this option is limited by the number of available processors.




**Learn more about** 

*	:ref:`option-ODHCPLEX-global_thread_limit` 



