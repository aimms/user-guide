.. _option-CPLEX-lower_objective_stop:


Lower Objective Stop
====================



:Type:	Floating point number	
:Range:	[-1e75, 1e75)	
:Default:	-1e75	



In a minimization MILP or MIQP, CPLEX will abort the optimization process as soon it finds a solution of value lower than or equal to the specified value for this option.



This option is ignored if the problem is multi-objective.



**Learn more about** 

*	:ref:`option-CPLEX-upper_objective_stop` 



