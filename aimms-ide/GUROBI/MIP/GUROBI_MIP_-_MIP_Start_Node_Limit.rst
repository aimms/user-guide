.. _option-GUROBI-mip_start_node_limit:


MIP Start Node Limit
====================



:Type:	Integer	
:Range:	{-2 .. 2000000000}	
:Default:	-1	



This option limits the number of branch-and-bound nodes explored when completing a partial MIP start. The default value of -1 uses the value of the **RINS Sub_MIP Node Limit**  option. A value of -2 shuts off MIP start processing entirely. Non-negative values are node limits.



**Note** 

*	MIP starts can also be used for NLP and MINLP models, and therefore this option also applies to these models.




**Learn more about** 

*	:ref:`option-GUROBI-mip_start` 
*	:ref:`option-GUROBI-rins_sub_mip_node_limit` 
