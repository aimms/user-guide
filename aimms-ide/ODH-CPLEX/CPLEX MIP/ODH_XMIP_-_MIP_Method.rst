.. _ODH-CPLEX_XMIP_-_MIP_Method:


MIP Method
==========



**Type**:	Selection	

**Range**:	The settings listed below	

**Default**:	Automatic	



This option can be used to set the algorithm to be used on subproblems. At the default setting, CPLEX decides which method will be used. Possible values are:



*	Automatic
*	Primal simplex
*	Dual simplex
*	Network simplex
*	Barrier
*	Sifting




With the setting "Sifting", CPLEX solves a sequence of LP subproblems, where the results from one subproblem are used to select columns from the original model for inclusion in the next subproblem. This iterative sifting process eventually converges to an optimal solution for the original model. Sifting is especially applicable to models with many more columns than rows.





**Note** 

*	The default 'Automatic' setting of this option currently selects the dual simplex optimizer for subproblems in a MIP or MIQP. The 'Automatic' setting may be expanded in the future so that CPLEX chooses the algorithm based on additional characteristics of the model.
*	The option **MIP Start Algorithm**  determines which algorithm is used to solve the initial relaxation of a MIP.




**Learn more about** 

*	:ref:`ODH-CPLEX_XMIP_-_MIP_Start_Algorit` 
