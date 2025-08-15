.. _ODH-CPLEX_XMIP_-_Select_Variables:


Select Variables
================



**Type**:	Selection	

**Range**:	The settings listed below	

**Default**:	Automatic	



The setting of this option is used to set the rule for selecting the branching variable at the node, which has been selected for branching. The maximum infeasibility rule chooses the variable with the largest fractional value; the minimum infeasibility rule chooses the variable with the smallest fractional value. The minimum infeasibility rule may lead more quickly to a first integer feasible solution, but will usually be slower overall to reach the optimal integer solution. The maximum infeasibility rule forces larger changes earlier in the tree, which tends to produce faster overall times to reach the optimal integer solution. Pseudo costs causes variable selection based on pseudo-costs which are derived from pseudo-shadow prices. Strong branching causes variable selection based on partially solving a number of subproblems which tentative branches to see which branch is the most promising. This strategy can be effective on large, difficult MIP problems. Pseudo-reduced costs are a computationally less intensive form of pseudo costs. The default value allows CPLEX to select the best rule based on the problem and its progress. Possible values are:



*	Min. infeasibility (branch on variable with min infeasibility)
*	Automatic
*	Max. infeasibility (branch on variable with max infeasibility)
*	Pseudo costs
*	Strong branching
*	Pseudo-reduced costs
