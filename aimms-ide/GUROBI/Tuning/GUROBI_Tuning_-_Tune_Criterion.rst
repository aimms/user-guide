.. _GUROBI_Tuning_-_Tune_Criterion:


Tune Criterion
==============



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Automatic	



This option modifies the tuning criterion for the tuning tool. Possible values are:



*	Automatic
*	Off
*	Optimality gap
*	Objective
*	Best solution




The primary tuning criterion is always to minimize the runtime required to find a proven optimal solution. However, for MIP models that don't solve to optimality within the specified time limit, a secondary criterion is needed. Set this option to 'Optimality gap' to use the optimality gap as the secondary criterion. Choose a value of 'Objective' to use the objective of the best feasible solution found. Choose a value of 'Best solution' to use the best objective bound. Choose 'Off' to ignore the secondary criterion and focus entirely on minimizing the time to find a proven optimal solution. The default value of 'Automatic' chooses automatically.





**Learn more about** 

*	:ref:`GUROBI_Tuning_Tool` 
