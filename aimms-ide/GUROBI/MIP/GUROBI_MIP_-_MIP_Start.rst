.. _option-GUROBI-mip_start:


MIP Start
=========



:Type:	Selection	
:Range:	The settings listed below	
:Default:	No	



This option determines whether Gurobi should load a start solution (if available) for solving a MIP model. Gurobi uses whatever start information is provided to try to construct a complete solution. Possible values are:



*	No
*	Yes




**Note** 

*	MIP starts can also be used for NLP and MINLP models.
*	Gurobi also supports :ref:`GUROBI_Multiple_MIP_Starts`.




**Learn more about** 

*	:ref:`option-GUROBI-mip_start_node_limit` 
*	:ref:`GUROBI_Multiple_MIP_Starts` 
