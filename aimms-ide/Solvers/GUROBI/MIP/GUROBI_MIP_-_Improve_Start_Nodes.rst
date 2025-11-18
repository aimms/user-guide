.. _option-GUROBI-improve_start_nodes:


Improve Start Nodes
===================



:Type:	Floating point number	
:Range:	[0.0,1e100]	
:Default:	1e100



The MIP solver can change option settings in the middle of the search in order to adopt a strategy that gives up on moving the best
bound and instead devotes all of its effort towards finding better feasible solutions. This option allows you to specify the node
count at which the MIP solver switches to a solution improvement strategy. For example, setting this option to 10 will cause the
MIP solver to switch strategies once the node count is larger than 10.



**Learn more about** 

*	:ref:`option-GUROBI-improve_start_gap`  
*	:ref:`option-GUROBI-improve_start_time`  
*	:ref:`option-GUROBI-improve_start_work`  
