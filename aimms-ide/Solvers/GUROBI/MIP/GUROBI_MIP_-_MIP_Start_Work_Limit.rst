.. _option-GUROBI-mip_start_work_limit:


MIP Start Work Limit
====================



:Type:	Floating point number	
:Range:	[0.0,1e100]	
:Default:	1e100



This option limits the total work (in work units) spent on completing a partial MIP start.

In contrast to the option **MIP Start Time Limit**, work limits are deterministic. This means that on the same hardware and with the same option
and attribute settings, a work limit will stop the optimization of a given model at the exact same point every time. One work unit
corresponds very roughly to one second on a single thread, but this greatly depends on the hardware on which Gurobi is running and
the model that is being solved.


**Note** 

*	MIP starts can also be used for NLP and MINLP models, and therefore this option also applies to these models.
*	This option was added in Gurobi 13.0.


**Learn more about** 

*	:ref:`option-GUROBI-mip_start` 
*	:ref:`option-GUROBI-mip_start_time_limit` 
*	:ref:`option-GUROBI-rins_sub_mip_node_limit` 
