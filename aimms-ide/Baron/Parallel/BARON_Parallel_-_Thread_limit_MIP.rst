

.. _Baron_Parallel_-_Thread_limit_MIP:


Thread limit MIP
================



**Type** :	Integer	

**Range** :	{1 .. 2100000000}	

**Default** :	1	



This option specifies the number of threads (or cores) BARON can use when solving problems with integer variables. For difficult problems with integer variables, most of BARON’s time is spent on solving MIP relaxations. Hence, considerable speedups may be obtained via parallel optimization of the MIP subproblems. By default, this option has the value of 1, meaning that a single thread (core) will be utilized.



