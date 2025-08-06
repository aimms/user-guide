.. _GUROBI_Parallel_-_Concurrent_MIP:


Concurrent MIP
==============



**Type** :	Integer	

**Range** :	{1 .. 2000000000}	

**Default** :	1	



This option enables the concurrent MIP solver. When the option is set to value n, the MIP solver performs n independent MIP solves in parallel, with different option settings for each. Optimization terminates when the first solve completes. By default, Gurobi chooses the option settings used for each independent solve automatically. The intent of concurrent MIP solving is to introduce additional diversity into the MIP search. This approach can sometimes solve models much faster than applying all available threads to a single MIP solve, especially on very large parallel machines.



The concurrent MIP solver divides available threads evenly among the independent solves. For example, if you have 6 threads available and you set this option to 2, the concurrent MIP solver will allocate 3 threads to each independent solve. Note that the number of independent solves launched will not exceed the number of available threads.



The total number of threads used by the concurrent MIP solver is limited by the option **Thread Limit** .



The concurrent MIP solver produces a slightly different log (as controlled by the option **Output File** ) from the standard MIP solver. Each concurrent MIP log line shows the objective for the best feasible solution found by any of the independent solves to that point, the best objective bound proved by any of the independent solves, and the relative gap between these two values.



If you switch on the option **Read Parameter File**  then you can specify multiple parameter files, one for each concurrent MIP solve, which allows you to choose your own option settings for each of the concurrent MIP solves. The Gurobi parameter file is explained in the help of the option **Read Parameter File** .



**Note** 

*	Information retrieved by callback procedures (solutions, objective bounds, etc.) will come from a single model.
*	User cutting planes are only applied to a single model.
*	You are not allowed to use lazy constraints with concurrent MIP, since they would only be applied to one model.




**Learn more about** 

*	:ref:`GUROBI_Logging_-_Output_File` 
*	:ref:`GUROBI_General_-_Read_Parameter_File` 
*	:ref:`GUROBI_Parallel_-_Thread_Limit` 



