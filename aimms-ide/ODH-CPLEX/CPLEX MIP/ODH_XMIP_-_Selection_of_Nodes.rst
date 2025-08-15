.. _ODH-CPLEX_XMIP_-_Selection_of_Nodes:


Selection of Nodes
==================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Best-bound	



The setting of this option is used to set the rule for selecting the next node to process when backtracking (proceeding back through the tree when a node is infeasible or cut off). The depth-first search strategy chooses the most recently created node. The best-bound strategy chooses the node with the best objective function for the associated LP relaxation. The best estimate strategy selects the node with the best estimate of the integer objective value that would be obtained from a node once all integer infeasibilities are removed. An alternate best-estimate search is also available. Possible values are:



*	Depth-first
*	Best-bound
*	Best-estimate
*	Alternate best-estimate



