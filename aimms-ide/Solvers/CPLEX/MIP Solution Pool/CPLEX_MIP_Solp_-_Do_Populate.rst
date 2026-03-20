.. _option-CPLEX-do_populate:


Do Populate
===========



:Type:	Selection	
:Range:	The settings listed below	
:Default:	No	



This option can be used to let CPLEX generate multiple solutions to a mixed integer programming (MIP) problem. Possible values are:

    *	No
    *	Yes


This option should be switched on before a normal solve statement (or before :any:`GMP::Instance::Solve`) to let CPLEX fill the solution pool.


**Note** 

*	If this option is switched on, no postsolve will be done, and sensitivity information and constraint level values will not be available.


**Learn more about** 

*	:doc:`CPLEX_Solution_Pool <../CPLEX_Solution_Pool>`  
*	:doc:`CPLEX_MIP_Solp_-_Pool_Abs_Obj_Gap <CPLEX_MIP_Solp_-_Pool_Abs_Obj_Gap>`  
*	:doc:`CPLEX_MIP_Solp_-_Pool_Intensity <CPLEX_MIP_Solp_-_Pool_Intensity>`  
*	:doc:`CPLEX_MIP_Solp_-_Pool_Rel_Obj_Gap <CPLEX_MIP_Solp_-_Pool_Rel_Obj_Gap>`  
*	:doc:`CPLEX_MIP_Solp_-_Pool_Repl_Strat <CPLEX_MIP_Solp_-_Pool_Repl_Strat>`  
*	:doc:`CPLEX_MIP_Solp_-_Populate_time_limit <CPLEX_MIP_Solp_-_Populate_time_limit>`  
*	:doc:`CPLEX_MIP_Solp_-_Population_Limit <CPLEX_MIP_Solp_-_Population_Limit>`  

