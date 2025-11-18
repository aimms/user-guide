.. _option-GUROBI-no_relaxation_heuristic_time:


No Relaxation Heuristic Time
============================



:Type:	Floating point number	
:Range:	[0,1e100]	
:Default:	0	



This option limits the amount of time (in seconds) spent in the No Relaxation heuristic. This heuristic searches for high-quality feasible solutions before solving the root relaxation. It can be quite useful on models where the root relaxation is particularly expensive.



Note that this option will introduce non-determinism - different runs may take different paths. Use the **No Relaxation Heuristic Work** option for deterministic results.



**Note** 

*	This option only affects MIP models.




**Learn more about** 

*	:ref:`option-GUROBI-no_relaxation_heuristic_work`  
