.. _option-ODHCPLEX-network_iterations:


Network Iterations
==================



:Type:	Integer	
:Range:	{0 .. 2147483647}	
:Default:	2147483647	



This option specifies the maximum number of iterations to be performed by the network optimizer before the algorithm terminates without reaching optimality.



**Note** 

*	This option is only active if one of the options **MIP Method**  or **MIP Start Algorithm**  is set to 'Network simplex'.




**Learn more about** 

*	:ref:`option-ODHCPLEX-mip_method`  
*	:ref:`option-ODHCPLEX-mip_start_algorithm`  
