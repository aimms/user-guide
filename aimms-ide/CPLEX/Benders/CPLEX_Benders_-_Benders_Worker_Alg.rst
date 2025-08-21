.. _option-CPLEX-benders_worker_algorithm:


Benders Worker Algorithm
========================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Automatic	



This option specifies which algorithm CPLEX should apply to solve subproblems of a Benders decomposition. At the default setting, CPLEX decides which method will be used. Possible values are:



*	Automatic
*	Primal simplex
*	Dual simplex
*	Network simplex
*	Barrier
*	Sifting




Given a formulation of a problem, CPLEX can decompose the model into a single master and possibly multiple subproblems (the worker or workers). This option designates the algorithm that CPLEX applies to solve the workers.





**Learn more about** 

*	:ref:`option-CPLEX-benders_strategy` 
