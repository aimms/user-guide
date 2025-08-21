.. _option-ODHCPLEX-number_of_repair_attempts:


Number of Repair Attempts
=========================



:Type: 	Integer
:Range: 	{-1 .. 2147483647}
:Default: 	-1



If you provide a MIP start (full or partial) solution that cannot be extended into a feasible solution, CPLEX will try to repair it. This option lets you indicate whether and how many times CPLEX should try to repair an infeasible MIP start. This option has no effect if the MIP start you supplied is feasible. It also has no effect if no MIP start was supplied. Possible values are:



-1:	None: do not try to repair	

0:	Automatic: let CPLEX choose	

n:	Indicates the frequency	



**Learn more about** 

*	:ref:`option-ODHCPLEX-advanced_start` 
