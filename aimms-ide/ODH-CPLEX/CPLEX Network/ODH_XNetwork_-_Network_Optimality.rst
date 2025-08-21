.. _option-ODHCPLEX-network_optimality:


Network Optimality
==================



:Type:	Floating point number	
:Range:	[1e-11, 1e-4]	
:Default:	1e-6	



The network optimality tolerance specifies the amount a reduced cost may violate the criterion for an optimal solution.



**Note** 

*	This option is only active if one of the options **MIP Method**  or **MIP Start Algorithm**  is set to 'Network simplex'.




**Learn more about** 

*	:ref:`option-ODHCPLEX-mip_method`  
*	:ref:`option-ODHCPLEX-mip_start_algorithm`  
