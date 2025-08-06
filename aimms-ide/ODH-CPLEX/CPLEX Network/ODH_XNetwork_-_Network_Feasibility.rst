.. _ODH-CPLEX_XNetwork_-_Network_Feasibility:


Network Feasibility
===================



**Type** :	Floating point number	

**Range** :	[1e-11, 1e-4]	

**Default** :	1e-6	



The network feasibility tolerance specifies the degree to which a problem's flow value may violate its bounds. This tolerance influences the selection of an optimal basis and can be reset to a lower value when a problem is having difficulty maintaining feasibility during optimization. You may also wish to lower this tolerance after finding an optimal solution if there is any doubt that the solution is truly optimal. If the feasibility tolerance is set too low, CPLEX may falsely conclude that a problem is infeasible. If you encounter reports of infeasibility during the optimization, a small adjustment in the feasibility tolerance may improve performance.



**Note** 

*	This option is only active if one of the options **MIP Method**  or **MIP Start Algorithm**  is set to 'Network simplex'.




**Learn more about** 

*	:ref:`ODH-CPLEX_XMIP_-_MIP_Method`  
*	:ref:`ODH-CPLEX_XMIP_-_MIP_Start_Algorit`  
