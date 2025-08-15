.. _ODH-CPLEX_XGeneral_-_Sifting_Algorithm:


Sifting Algorithm
=================



**Type**:	Selection	

**Range**:	The settings listed below	

**Default**:	Automatic	



This option sets the algorithm to be used for solving sifting subproblems. Possible values are:



*	Automatic
*	Primal simplex
*	Dual simplex
*	Network simplex
*	Barrier




Sifting solves a sequence of LP subproblems, where the results from one subproblem are used to select columns from the original model for inclusion in the next subproblem. This iterative sifting process eventually converges to an optimal solution for the original model. Sifting is especially applicable to models with many more columns than rows.





At the default setting CPLEX chooses the optimizer automatically, typically switching between barrier and primal simplex as the optimization proceeds.





Sifting can be selected for solving LP and MIP models using the following options: **MIP Method** , **MIP Start Algorithm** , **SubMIP Start Algorithm**  and **SubMIP Subproblem Algorithm** .





**Learn more about** 

*	:ref:`ODH-CPLEX_XMIP_-_MIP_Method`  
*	:ref:`ODH-CPLEX_XMIP_-_MIP_Start_Algorit` 
*	:ref:`ODH-CPLEX_XMIP_Advanced_-_SubMIP_Start_Algorithm`
*	:ref:`ODH-CPLEX_XMIP_Advanced_-_SubMIP_Subproblem_Algorithm`



