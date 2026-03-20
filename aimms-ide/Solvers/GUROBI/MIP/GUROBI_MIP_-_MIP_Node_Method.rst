.. _option-GUROBI-mip_node_method:


MIP Node Method
===============



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Automatic	



This option determines which algorithm should be used to solve MIP node relaxations. Possible values are:



    *	Automatic
    *	Primal simplex
    *	Dual simplex
    *	Barrier




At the default value Gurobi chooses automatically. Barrier is not an option for MIQP node relaxations.





**Note** 

*	The option **Method**  determines which algorithm should be used when solving the root node of a MIP model.




**Learn more about** 

*	:doc:`GUROBI_General_-_Method <../General/GUROBI_General_-_Method>` 
