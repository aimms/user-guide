.. _option-CPLEX-local_branching_heuristic:


Local Branching Heuristic
=========================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	No	



This option lets you control whether CPLEX applies a local branching heuristic to try to improve new incumbents found during a MIP search. By default, it is turned off. If you turn it on, CPLEX will invoke a local branching heuristic only when it finds a new incumbent. If CPLEX finds multiple incumbents at a single node, the local branching heuristic will be applied only to the last one found. Possible values are:



*	No
*	Yes



