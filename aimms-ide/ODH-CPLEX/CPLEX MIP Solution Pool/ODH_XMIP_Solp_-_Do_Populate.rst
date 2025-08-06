.. _ODH-CPLEX_XMIP_Solp_-_Do_Populate:


Do Populate
===========



**Type** :	Selection	

**Range** :	The settings listed below	

**Default** :	No	



This option can be used to let CPLEX generate multiple solutions to a mixed integer programming (MIP) problem. Possible values are:



*	No
*	Yes




This option should be switched on before a normal solve statement (or before GMP::Instance::Solve) to let CPLEX fill the solution pool.





**Note** 

*	If this option is switched on, no postsolve will be done, and sensitivity information and constraint level values will not be available.




**Learn more about** 

*	:ref:`ODH-CPLEX_XMIP_Solp_-_Pool_Abs_Obj_Gap`  
*	:ref:`ODH-CPLEX_XMIP_Solp_-_Pool_Intensity`  
*	:ref:`ODH-CPLEX_XMIP_Solp_-_Pool_Rel_Obj_Gap`  
*	:ref:`ODH-CPLEX_XMIP_Solp_-_Pool_Repl_Strat`  
*	:ref:`ODH-CPLEX_XMIP_Solp_-_Populate_time_limit`  
*	:ref:`ODH-CPLEX_XMIP_Solp_-_Population_Limit`  



