.. _option-GUROBI-mip_start_time_limit:


MIP Start Time Limit
====================



:Type:	Floating point number	
:Range:	[0.0,1e100]	
:Default:	1e100



This option limits the total time (in seconds) spent on completing a partial MIP start.

Note that this parameter will introduce non-determinism - different runs may take different paths. Use the option **MIP Start Work Limit**
for deterministic results.


**Note** 

*	MIP starts can also be used for NLP and MINLP models, and therefore this option also applies to these models.
*	This option was added in Gurobi 13.0.


**Learn more about** 

*	:ref:`option-GUROBI-mip_start` 
*	:ref:`option-GUROBI-mip_start_work_limit` 
*	:ref:`option-GUROBI-rins_sub_mip_node_limit` 
