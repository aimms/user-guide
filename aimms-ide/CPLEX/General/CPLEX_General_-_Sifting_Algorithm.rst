.. _CPLEX_General_-_Sifting_Algorithm:


Sifting Algorithm
=================



**Type** :	Selection	

**Range** :	The settings listed below	

**Default** :	Automatic	



This option sets the algorithm to be used for solving sifting subproblems. Possible values are:



*	Automatic
*	Primal simplex
*	Dual simplex
*	Network simplex
*	Barrier




Sifting solves a sequence of LP subproblems, where the results from one subproblem are used to select columns from the original model for inclusion in the next subproblem. This iterative sifting process eventually converges to an optimal solution for the original model. Sifting is especially applicable to models with many more columns than rows.





At the default setting CPLEX chooses the optimizer automatically, typically switching between barrier and primal simplex as the optimization proceeds. It is recommended that you do not turn off the barrier crossover step, by setting the option **Solution Type**  to 'Nonbasic', when you use the sifting optimizer, so that CPLEX can carry out this switching as needed.





Sifting can be selected for solving LP and MIP models using the following options: **LP Method** , **MIP Method** , **MIP Start Algorithm** , **SubMIP Start Algorithm** , **SubMIP Subproblem Algorithm** , and **Benders Worker Algorithm** .





**Learn more about** 

*	:ref:`CPLEX_Benders_-_Benders_Worker_Alg`  
*	:ref:`CPLEX_General_-_LP_Method`  
*	:ref:`CPLEX_MIP_-_MIP_Method`  
*	:ref:`CPLEX_MIP_-_MIP_Start_Algorit` 
*	:ref:`CPLEX_General_-_Solution_Type` 
*	:ref:`CPLEX_MIP_Advanced_-_SubMIP_Start_Algorithm` 
*	:ref:`CPLEX_MIP_Advanced_-_SubMIP_Subproblem_Algorithm` 



