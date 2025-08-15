.. _GUROBI_Solution_Pool_-_Pool_Gap:


Pool Gap
========



:Type:	Floating point number	
:Range:	[0,1e100]	
:Default:	1e100



This option determines the maximum gap for stored solutions. When this option is set to a non-default value, solutions whose objective values exceed that of the best known solution by more than the specified (relative) gap are discarded. For example, if the MIP solver has found a solution at objective 100, then a setting of 0.2 would discard solutions with objective worse than 120 (assuming a minimization objective).



**Note** 

*	This option only affects mixed integer programming (MIP) models.




**Learn more about** 

*	:ref:`GUROBI_Solution_Pool_-_Pool_Absolute_Gap` 
