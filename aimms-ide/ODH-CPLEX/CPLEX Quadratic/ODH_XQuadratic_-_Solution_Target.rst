.. _ODH-CPLEX_XQuadratic_-_Solution_Target:


Solution Target
===============



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Automatic	



This option specifies the type of solution CPLEX attempts to compute when CPLEX solves a, possibly, nonconvex continuous quadratic model (QP) or mixed integer quadratic model (MIQP). In other words, the variables of the model can be continuous or mixed integer and continuous; the objective function includes a quadratic term, and the objective function is not positive semi-definite (non PSD). Possible values are:



*	Automatic
*	Search for convex optimum
*	Search for local optimum
*	Search for global optimum




By default, CPLEX first attempts to compute a provably optimal solution. If CPLEX cannot compute a provably optimal solution because the objective function is not convex, CPLEX will return an error. 





When this option is set to 'Search for convex optimum', CPLEX searches for a globally optimal solution to a convex model.





When this option is set to 'Search for local optimum', CPLEX first attempts to compute a provably optimal solution. If CPLEX cannot compute a provably optimal solution because the objective function is not convex, CPLEX searches for a solution that satisfies first-order optimality conditions but is not necessarily globally optimal. In such a case, you can query the solution status to determine the kind of solution CPLEX found.





When this option is set to 'Search for global optimum', if the problem type is QP, CPLEX first changes the problem type to MIQP. CPLEX then solves the problem (whether originally QP or MIQP) to global optimality.





**Learn more about** 

*	:ref:`ODH-CPLEX_XCuts_-_Clique_Cuts` 
*	:ref:`ODH-CPLEX_XCuts_-_RLT_Cuts` 
