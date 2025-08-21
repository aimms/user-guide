.. _option-CPLEX-pool_capacity:


Pool Capacity
=============



:Type:	Integer	
:Range:	{0 .. 2100000000}	
:Default:	2100000000	



This option limits the number of solutions kept in the solution pool. Superfluous solutions are managed according to the replacement strategy set by the option **Pool Replacement Strategy** . A value of 0 turns off all features of the solution pool.



This option has only meaning if the option **Do** **Populate**  is switched on.



**Learn more about** 

*	:ref:`option-CPLEX-do_populate`  
*	:ref:`option-CPLEX-pool_replacement_strategy`  
