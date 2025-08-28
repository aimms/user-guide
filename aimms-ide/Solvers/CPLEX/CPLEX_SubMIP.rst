.. _CPLEX_SubMIP:


SubMIP
======

In CPLEX, a subMIP is an auxiliary mixed integer program (MIP). A subMIP is not a subproblem. (A subproblem is the LP relaxation of a node other than the root.) 



CPLEX solves subMIPs in these situations:




    *   when it builds a solution from a partial MIP start;
    *   when it repairs an infeasible MIP start; 
    *   when it executes the relaxation induced neighborhood search (RINS) heuristic; 
    *   when it branches locally;
    *   when it polishes a solution. 



A subMIP is usually smaller in size than the MIP that CPLEX is currently solving. CPLEX conventionally solves a subMIP with stricter limits on
resources than in the original problem, but CPLEX offers options that enable you to specify other choices:




    *   **SubMIP Start Algorithm**: algorithm for initial MIP relaxation of a subMIP of a MIP 
    *   **SubMIP Subproblem Algorithm**: algorithm for subproblems of a subMIP of a MIP 
    *   **SubMIP Scale**: scale option for subMIPs 
    *   **SubMIP Node Limit**: limit on nodes explored when CPLEX solves a subMIP



**Learn more about** 

*	:ref:`option-CPLEX-submip_node_limit`  
*	:ref:`option-CPLEX-submip_scale`  
*	:ref:`option-CPLEX-submip_start_algorithm`  
*	:ref:`option-CPLEX-submip_subproblem_algorithm`  
