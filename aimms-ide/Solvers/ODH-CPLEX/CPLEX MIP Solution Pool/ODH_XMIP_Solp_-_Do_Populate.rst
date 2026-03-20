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

*	:doc:`ODH_XMIP_Solp_-_Pool_Abs_Obj_Gap`  
*	:doc:`ODH_XMIP_Solp_-_Pool_Intensity`  
*	:doc:`ODH_XMIP_Solp_-_Pool_Rel_Obj_Gap`  
*	:doc:`ODH_XMIP_Solp_-_Pool_Repl_Strat`  
*	:doc:`ODH_XMIP_Solp_-_Populate_time_limit`  
*	:doc:`ODH_XMIP_Solp_-_Population_Limit`  



