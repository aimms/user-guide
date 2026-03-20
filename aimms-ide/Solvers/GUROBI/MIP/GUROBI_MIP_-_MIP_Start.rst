.. _option-GUROBI-mip_start:


MIP Start
=========



:Type:	Selection	
:Range:	The settings listed below	
:Default:	No	



This option determines whether Gurobi should load a start solution (if available) for solving a MIP model. Gurobi uses whatever
start information is provided to try to construct a complete solution. Possible values are:

    *	No
    *	Yes


**Note** 

*	MIP starts can also be used for NLP and MINLP models.
*	Gurobi also supports :doc:`../GUROBI_Multiple_MIP_Starts`.
*	Gurobi can write the (first) MIP start to a file if the option **Restart** is set to 'Before'.


**Learn more about** 

*	:doc:`GUROBI_MIP_-_MIP_Start_Node_Limit` 
*	:doc:`GUROBI_MIP_-_MIP_Start_Time_Limit` 
*	:doc:`GUROBI_MIP_-_MIP_Start_Work_Limit` 
*	:doc:`../General/GUROBI_General_-_Restart` 
*	:doc:`../GUROBI_Multiple_MIP_Starts` 
