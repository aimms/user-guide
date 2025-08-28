.. _option-ODHCPLEX-do_populate:


Do Populate
===========



:Type:	Selection	
:Range:	The settings listed below	
:Default:	No	



This option can be used to let CPLEX generate multiple solutions to a mixed integer programming (MIP) problem. Possible values are:



    *	No
    *	Yes




This option should be switched on before a normal solve statement (or before GMP::Instance::Solve) to let CPLEX fill the solution pool.





**Note** 

*	If this option is switched on, no postsolve will be done, and sensitivity information and constraint level values will not be available.




**Learn more about** 

*	:ref:`option-ODHCPLEX-pool_absolute_objective_gap`  
*	:ref:`option-ODHCPLEX-pool_intensity`  
*	:ref:`option-ODHCPLEX-pool_relative_objective_gap`  
*	:ref:`option-ODHCPLEX-pool_replacement_strategy`  
*	:ref:`option-ODHCPLEX-populate_time_limit`  
*	:ref:`option-ODHCPLEX-population_limit`  



