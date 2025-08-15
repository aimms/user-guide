.. _CPLEX_MIP_Solp_-_Pool_Capacity:


Pool Capacity
=============



:Type:	Integer	
:Range:	{0 .. 2100000000}	
:Default:	2100000000	



This option limits the number of solutions kept in the solution pool. Superfluous solutions are managed according to the replacement strategy set by the option **Pool Replacement Strategy** . A value of 0 turns off all features of the solution pool.



This option has only meaning if the option **Do** **Populate**  is switched on.



**Learn more about** 

*	:ref:`CPLEX_MIP_Solp_-_Do_Populate`  
*	:ref:`CPLEX_MIP_Solp_-_Pool_Repl_Strat`  
