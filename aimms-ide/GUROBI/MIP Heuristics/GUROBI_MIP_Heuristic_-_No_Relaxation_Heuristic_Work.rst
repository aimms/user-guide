.. _GUROBI_MIP_Heuristic_-_No_Relaxation_Heuristic_Work:


No Relaxation Heuristic Work
============================



:Type:	Floating point number	
:Range:	[0,1e100]	
:Default:	0	



This option limits the amount of work spent in the No Relaxation heuristic. This heuristic searches for high-quality feasible solutions before solving the root relaxation. It can be quite useful on models where the root relaxation is particularly expensive.



The work metric used in this option is tough to define precisely. A single unit corresponds to roughly a second, but this will depend on the machine, the core count, and in some cases the model. You may need to experiment to find a good setting for your model.



**Note** 

*	This option only affects MIP models.




**Learn more about** 

*	:ref:`GUROBI_MIP_Heuristic_-_No_Relaxation_Heuristic_Time`  
