.. _GUROBI_MIP_-_Select_Variables:


Select Variables
================



**Type** :	Selection	

**Range** :	The settings listed below	

**Default** :	Automatic	



The option controls the branch variable selection strategy. The default setting makes an automatic choice, depending on problem characteristics. Possible values are:



*	Automatic
*	Pseudo reduced cost branching
*	Pseudo shadow price branching
*	Maximum infeasibility branching
*	Strong branching




Strong branching causes variable selection based on partially solving a number of subproblems which tentative branches to see which branch is the most promising. This strategy can be effective on large, difficult MIP problems.

