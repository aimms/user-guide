.. _option-CPLEX-benders_strategy:


Benders Strategy
================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Off	



This option determines whether CPLEX should use the :ref:`option-CPLEX-benders_decomposition`  algorithm for solving a problem, and how the model should be decomposed. Given a formulation of a problem, CPLEX can decompose the model into a single master and (possibly multiple) subproblems. For certain type of problems, using multiple subproblems offers significant performance improvements because they can be solved in parallel. For MIP problems, under certain conditions, CPLEX can apply Benders decomposition to improve the search to find more feasible solutions more quickly. Possible values are:



*	Off
*	User
*	Worker
*	Full




With this option, you can direct CPLEX to decompose your model and to apply its implementation of the Benders decomposition algorithm in one of these alternative strategies:




*	**User** : CPLEX attempts to decompose your model strictly according to the decomposition specified by you.



*	**Worker** : CPLEX decomposes your model by using the decomposition specified by you as hints and refining the decomposition where it can.




		„ CPLEX initially decomposes your model according to your specification.





		„ CPLEX then attempts to refine that decomposition by further decomposing the specified subproblems.




*	**Full** : CPLEX automatically decomposes your model, ignoring any specification you may have supplied. 




		„ CPLEX puts all integer variables into the master. 





		„ CPLEX puts all continuous variables into a subproblem. 





		„ CPLEX further decomposes that subproblem, if possible.





The strategies 'User' and 'Worker' require you to specify a decomposition; see the section :ref:`option-CPLEX-benders_decomposition`  for more information.





The strategy 'Full' can only be applied to MIP problems.





**Note** 

*	CPLEX only supports Benders decomposition for linear problems.
*	CPLEX does not support Benders decomposition for problems with ranged, indicator, SOS or lazy constraints.
*	CPLEX does not support Benders decomposition for multi-objective optimization problems.
*	The strategies 'User' and 'Worker' require you to use GMP functionality (see the section :ref:`option-CPLEX-benders_decomposition` ). The strategy 'Full' can also be applied to a normal solve-statement.




**Learn more about** 

*	:ref:`option-CPLEX-benders_decomposition` 



