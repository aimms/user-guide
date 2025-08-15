.. _ODH-CPLEX_XMIP_Solp_-_Pool_Repl_Strat:


Pool Replacement Strategy
=========================



**Type**:	Selection	

**Range**:	The settings listed below	

**Default**:	FIFO	



This option designates the strategy for replacing a solution in the solution pool when the solution pool has reached its capacity. Possible values are:



*	FIFO
*	Worst objective
*	Diverse solutions




The value default value of 'FIFO' replaces solutions according to a first-in, first-out policy. The value 'Worst objective' keeps the solutions with the best objective values. The value 'Diverse solutions' replaces solutions in order to build a set of diverse solutions. 





If the solutions you obtain are too similar to each other, try setting 'Diverse solutions'. 





This option has only meaning if the option **Do Populate**  is switched on.





**Learn more about** 

*	:ref:`ODH-CPLEX_XMIP_Solp_-_Do_Populate`  



