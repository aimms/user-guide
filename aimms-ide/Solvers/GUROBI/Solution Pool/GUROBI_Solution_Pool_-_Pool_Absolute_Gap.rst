.. _option-GUROBI-pool_absolute_gap:


Pool Absolute Gap
=================



:Type:	Floating point number	
:Range:	[0,1e100]	
:Default:	1e100



This option determines how large a (absolute) gap to tolerate in stored solutions. When this option is set to a non-default value, solutions whose objective values exceed that of the best known solution by more than the specified (absolute) gap are discarded. For example, if the MIP solver has found a solution at objective 100, then an absolute gap setting of 20 would discard solutions with objective worse than 120 (assuming a minimization objective).



**Note** 

*	This option only affects mixed integer programming (MIP) models.




**Learn more about** 

*	:ref:`option-GUROBI-pool_gap` 
