.. _option-ODHCPLEX-recurse:


Recurse
=======



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Off	



This option specifies can be used to active the recurse using heuristic to solve sub-models when a feasible solution has been obtained. Possible values are:



*	All threads for infeasible solution
*	Odd numbered threads for infeasible solution
*	One thread only for infeasible solution
*	Off
*	One thread only
*	Odd numbered threads
*	All threads




By default this option is switched off which means that CPLEX is used for solving sub-models.




