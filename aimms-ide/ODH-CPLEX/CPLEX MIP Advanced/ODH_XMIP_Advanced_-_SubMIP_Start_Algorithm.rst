.. _ODH-CPLEX_XMIP_Advanced_-_SubMIP_Start_Algorithm:


SubMIP Start Algorithm
======================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Standard	



This option sets which continuous optimizer will be used to solve the initial relaxation of a subMIP of a MIP. Possible values are:



*	Automatic
*	Primal simplex
*	Dual simplex
*	Network simplex
*	Barrier
*	Sifting




SubMIPS are described in the section 'SubMIP' of the CPLEX 20.1 help.





The default 'Automatic' setting of this option currently selects the concurrent optimizer for root relaxations of mixed integer linear programming models (MILP) and selects the dual simplex optimizer for root relaxations of mixed integer quadratic programming models (MIQP).





For MILP (integer constraints and otherwise continuous variables), all settings are permitted. 





For MIQP (integer constraints and positive semi-definite quadratic terms in the objective), settings 'Sifting' and 'Concurrent' are not implemented; if you happen to choose them, setting 'Sifting' reverts to 'Automatic' and setting 'Concurrent' reverts to 'Barrier'. 





For MIQCP (integer constraints and positive semi-definite quadratic terms among the constraints), only the setting 'Automatic' is permitted.





Sifting solves a sequence of LP subproblems, where the results from one subproblem are used to select columns from the original model for inclusion in the next subproblem. This iterative sifting process eventually converges to an optimal solution for the original model. Sifting is especially applicable to models with many more columns than rows.





**Note** 

*	This rarely used option is helpful **only**  in rare "corner" cases where there is clear evidence that the default choice of the continuous optimizer is really inappropriate for the heuristics applied to the problem.



