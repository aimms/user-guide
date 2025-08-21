.. _option-CPLEX-submip_subproblem_algorithm:


SubMIP Subproblem Algorithm
===========================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Automatic	



This option decides which continuous optimizer will be used to solve the subproblems of a subMIP in a MIP, after the initial relaxation. Possible values are:



*	Automatic
*	Primal simplex
*	Dual simplex
*	Network simplex
*	Barrier
*	Sifting




SubMIPS are described in the section :ref:`option-CPLEX-submip` .





The default 'Automatic' setting of this option currently selects the dual simplex optimizer for subproblem solution for MILP and MIQP.





For MILP (integer constraints and otherwise continuous variables), all settings are permitted. 





For MIQP (integer constraints and positive semi-definite quadratic terms in the objective), setting 'Network' is not permitted, and setting 'Sifting' reverts to 'Automatic'. 





For MIQCP (integer constraints and positive semi-definite quadratic terms among the constraints), only the setting 'Automatic' is permitted. In other words, given a problem of type MIQCP, and any setting of this option other than 'Automatic', CPLEX will exit because of the quadratic constraint or quadratic constraints, and CPLEX displays an error message specifying that a mixed integer problem cannot be solved by this setting. 





With the setting 'Sifting', CPLEX solves a sequence of LP subproblems, where the results from one subproblem are used to select columns from the original model for inclusion in the next subproblem. This iterative sifting process eventually converges to an optimal solution for the original model. Sifting is especially applicable to models with many more columns than rows.





**Note** 

*	This rarely used option is helpful **only**  in rare "corner" cases where there is clear evidence that the default choice of the continuous optimizer is really inappropriate for the heuristics applied to the problem.




**Learn more about** 

*	:ref:`option-CPLEX-submip` 
