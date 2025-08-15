.. _KNITRO_Advanced_-_LP_Algorithm:


LP Algorithm
============



:Type:	Selection	
:Range:	The settings listed below	
:Default:	AIMMS computes	



This option indicates which algorithm to use to solve linear programming (LP) subproblems when using the Knitro Active Set or SQP algorithms. Possible values are:



*	Automatic
*	Primal simplex
*	Dual simplex
*	Barrier




This option is currently only active when using the CPLEX LP solver chosen via the option **LP Solver** .





This option has no effect on the Interior/Direct and Interior/CG algorithms.





**Learn more about** 

*	:ref:`KNITRO_General_-_LP_Solver` 
