.. _KNITRO_IP_-_Barrier_Penalty_Constraint_St:


Barrier Penalty Constraint Strategy
===================================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Automatic	



This option indicates whether a penalty approach is applied to the constraints. Using a penalty approach may be helpful when the problem has degenerate or difficult constraints. It may also help to more quickly identify infeasible problems, or achieve feasibility in problems with difficult constraints. Possible values are:



*	Automatic
*	No constraints penalized
*	All constraints penalized
*	Equalities penalized




This option may be used to apply a special penalty method to the constraints. This can improve performance on problems with degenerate constraints or problems where Knitro is struggling to get feasible.





This option has no effect on the Active Set and SQP algorithms.





**Learn more about** 

*	:ref:`KNITRO_General_-_Algorithm` 
