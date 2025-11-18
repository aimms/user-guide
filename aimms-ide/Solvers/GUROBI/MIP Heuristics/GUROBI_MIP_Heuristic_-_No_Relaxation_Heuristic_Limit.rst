.. _option-GUROBI-no_relaxation_heuristic_time:


No Relaxation Heuristic Time
============================



:Type:	Integer	
:Range:	{0 .. 2000000000}	
:Default:	2000000000



This option limits the number of solutions found by the No Relaxation heuristic. This heuristic searches for high-quality feasible
solutions before solving the root relaxation. It can be quite useful on models where the root relaxation is particularly expensive.


**Note** 

*	This option only affects MIP models.


**Learn more about** 

*	:ref:`option-GUROBI-no_relaxation_heuristic_work`  
