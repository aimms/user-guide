.. _GUROBI_MIP_-_MIP_Node_Method:


MIP Node Method
===============



**Type** :	Selection	

**Range** :	The settings listed below	

**Default** :	Automatic	



This option determines which algorithm should be used to solve MIP node relaxations. Possible values are:



*	Automatic
*	Primal simplex
*	Dual simplex
*	Barrier




At the default value Gurobi chooses automatically. Barrier is not an option for MIQP node relaxations.





**Note** 

*	The option **Method**  determines which algorithm should be used when solving the root node of a MIP model.




**Learn more about** 

*	:ref:`GUROBI_General_-_Method` 
