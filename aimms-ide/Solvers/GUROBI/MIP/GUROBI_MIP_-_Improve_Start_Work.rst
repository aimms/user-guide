.. _option-GUROBI-improve_start_work:


Improve Start Work
==================



:Type:	Floating point number	
:Range:	[0.0,1e100]	
:Default:	1e100



The MIP solver can change option settings in the middle of the search in order to adopt a strategy that gives up on moving the best bound
and instead devotes all of its effort towards finding better feasible solutions. This option allows you to specify the work (in work
units) when the MIP solver switches to this solution improvement strategy. For example, setting this option to 10 will cause the MIP
solver to switch strategies 10 work units after starting the optimization, provided that at least one feasible solution has been found.
If no incumbent solution exists when the specified work is reached, the strategy switch will occur as soon as the first feasible solution
is discovered.


**Note** 

*	This option was added in Gurobi 13.0.


**Learn more about** 

*	:ref:`option-GUROBI-improve_start_gap`  
*	:ref:`option-GUROBI-improve_start_nodes`  
*	:ref:`option-GUROBI-improve_start_time`  
