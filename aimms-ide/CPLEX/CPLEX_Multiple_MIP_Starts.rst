.. _CPLEX_Multiple_MIP_Starts:

Multiple MIP Starts
===================

CPLEX supports multiple MIP starts; that is, a user may maintain more than one starting solution with values for continuous and discrete variables for CPLEX to use as an advanced starting point. MIP starts are also known as advanced starts or warm starts.

A solution in the solution repository can be marked as a MIP start by using the AIMMS routine GMP::Solution::SetMIPStartFlag. For example, to mark the solutions 2 and 3 in the solution repository of a mathematical program 'MP' and solve the MIP use

	gmpMP := GMP::Instance::Generate( MP );

	GMP::Solution::SetMIPStartFlag( gmpMP, 2, 1 );

	GMP::Solution::SetMIPStartFlag( gmpMP, 3, 1 );

	GMP::Instance::Solve( gmpMP );

where 'gmpMP' is an element parameter with range 'AllGeneratedMathematicalPrograms'.

Users may want CPLEX to process multiple MIP starts differently, expending more effort on some than on others. Moreover, a user may want to limit the effort CPLEX applies to MIP starts when it transforms each MIP start into a feasible solution, especially if there are many of them. In that context, the user may specify a level of effort that CPLEX should expend for each MIP start to transform it into a feasible solution. The user specifies the level of effort by using the optional argument 'effortLevel' in the AIMMS routine GMP::Solution::SetMIPStartFlag.



CPLEX applies the effort level specified by the user. If a MIP start does not contain enough information to be processed with the effort level specified by the user, then CPLEX will not process this MIP start. For example, if the MIP start does not specify values for all variables but the user has specified an effort level to check feasibility, CPLEX does not process the MIP start. 



Here are the levels of effort and their effect:




*   Level 0 (the default): CPLEX expends effort at level 4 for the first MIP start (which will be the incumbent after a MIP optimization or a call to populate) and at level 1 for all other MIP starts. 




*   Level 1: CPLEX checks feasibility of the corresponding MIP start. This level requires the user to provide values for all variables in the problem, both discrete and continuous. If any values are missing, CPLEX does not process this MIP start. 




*   Level 2: CPLEX solves the fixed LP problem specified by the MIP start. This effort level requires the user to provide values for all discrete variables. If values for any discrete variables are missing, CPLEX does not process the MIP start. 




*   Level 3: CPLEX solves a subMIP. The user must specify the value of at least one discrete variable at this effort level. CPLEX uses the values of continuous variables at this effort level only in the initial phase when it attempts to determine values for unspecified discrete variables. 




*   Level 4: CPLEX attempts to repair the MIP start if it is infeasible, according to the option **Number of Repair Attempts**  that sets the frequency to try to repair infeasible MIP start. The user must specify the value of at least one discrete variable at this effort level, too.



A user may specify a different level of effort for each MIP start, for example, different effort levels for the incumbent, for a MIP start corresponding to a solution in the solution repository, for a MIP start supplied by the user.



**Note** 

*	The option **Advanced Start**  can be used if only one MIP start is available.




**Learn more about** 

*	Search for GMP::Solution::SetMIPStartFlag (Function Reference)
*	:ref:`CPLEX_General_-_AdvancedStart` 
*	:ref:`CPLEX_MIP_-_NumberofRepairAttempts`  



