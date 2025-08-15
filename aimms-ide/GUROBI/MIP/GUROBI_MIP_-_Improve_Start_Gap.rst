.. _GUROBI_MIP_-_Improve_Start_Gap:


Improve Start Gap
=================



:Type:	Floating point number	
:Range:	[0.0,1e100]	
:Default:	0.0



The MIP solver can change option settings in the middle of the search in order to adopt a strategy that gives up on moving the best bound and instead devotes all of its effort towards finding better feasible solutions. This option allows you to specify an optimality gap at which the MIP solver will switch to this strategy. For example, setting this option to 0.1 will cause the MIP solver to switch once the relative optimality gap is smaller than 0.1.



**Learn more about** 

*	:ref:`GUROBI_MIP_-_Improve_Start_Nodes`  
*	:ref:`GUROBI_MIP_-_Improve_Start_Time`  
