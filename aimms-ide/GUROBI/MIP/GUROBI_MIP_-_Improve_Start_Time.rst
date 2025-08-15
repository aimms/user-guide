.. _GUROBI_MIP_-_Improve_Start_Time:


Improve Start Time
==================



:Type:	Floating point number	
:Range:	[0.0,1e100]	
:Default:	1e100



The MIP solver can change option settings in the middle of the search in order to adopt a strategy that gives up on moving the best bound and instead devotes all of its effort towards finding better feasible solutions. This option allows you to specify a time limit when the MIP solver will switch to this strategy. For example, setting this option to 10 will cause the MIP solver to switch 10 seconds after starting the optimization.



**Learn more about** 

*	:ref:`GUROBI_MIP_-_Improve_Start_Gap`  
*	:ref:`GUROBI_MIP_-_Improve_Start_Nodes`  
