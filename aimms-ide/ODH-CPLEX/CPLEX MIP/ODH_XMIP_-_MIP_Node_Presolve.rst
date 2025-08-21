.. _option-ODHCPLEX-mip_node_presolve:


MIP Node Presolve
=================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Automatic	



This option indicates whether node presolve should be performed at the nodes of a mixed integer programming solution. Node presolve can significantly reduce solution time for some models. The defaults setting ("Automatic") is generally effective at determining whether to apply node presolve, although runtimes can be reduced for some models by turning node presolve off. Possible values are:



*	No node presolve
*	Automatic
*	Force node presolve
*	Probe integer-infeasible variables
*	Aggressive node probing



