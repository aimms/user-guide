.. _option-CPLEX-print_presolve_status:


Print Presolve Status
=====================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	No	



This option indicates whether presolve status information for the variables and constraint should be printed to the listing file. Possible values are:



    *	No
    *	Yes




Possible presolve statuses for the variables are:




*	In presolved problem
*	Fixed to lower bound
*	Fixed to upper bound
*	Fixed to other value
*	Aggregated out
*	Deleted or merged




Possible presolve statuses for the constraints are:




*	In presolved problem
*	Redundant
*	Used for aggregation
*	Deleted




This option is especially useful to detect which constraints with a Big M value are not eliminated by preprocessing. A Big M constraint that is not eliminated by preprocessing can be reformulated as an Indicator Constraint.





**Note** 

*	Presolve status information is only available for LP and MIP models.
*	Presolve status information is not available if CPLEX Presolve detects that the model is infeasible or unbounded.
*	Presolve status information is not available if the procedure GMP::SolverSession::Execute or GMP::SolverSession::AsynchronousExecute is used to solve the model.




**Learn more about** 

*	 :ref:`CPLEX_Indicator_Constraints` 



