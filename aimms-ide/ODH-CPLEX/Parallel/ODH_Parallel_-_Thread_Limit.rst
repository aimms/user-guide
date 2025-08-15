.. _ODH-CPLEX_Parallel_-_Thread_Limit:


Thread Limit
============



:Type:	Integer	
:Range:	{-1 .. 1024}	
:Default:	-1



This option determines the number of heuristic threads used by ODH-CPLEX. Values are:



   -1 = automatically determined

   0 = run in serial mode

   >0 = use the specified number of threads



At the default value of -1, the total number of threads allocated for ODH-CPLEX is set to the number of physical processors available on the computer.



**Remark** 

As ODH-CPLEX must use separate threads for the main CPLEX solve and for the ODH engine if the option **Search Mode**  equals 'Optimal solution', ODH-CPLEX needs to use at least 2 threads. For that reason, with **Search Mode**  equal to 'Optimal solution', if this option is set to 0 or 1 then 2 threads will be used; one by the main CPLEX solve and one by the ODH engine.



**Learn more about** 

*	:ref:`ODH-CPLEX_-_Parallel_Execution` 
