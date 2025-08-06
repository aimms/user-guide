.. _GUROBI_MIP_Presolve_-_Presolve_Sparsify_Reduction:


Presolve Sparsify Reduction
===========================



**Type** :	Selection	

**Range** :	The settings listed below	

**Default** :	Automatic	



This option controls the presolve sparsify reduction for MIP models. This reduction can sometimes significantly reduce the number of nonzero values in the presolved model. Possible values are:



*	Automatic
*	Off
*	MIP only
*	Always




Value 'Off' shuts off the reduction, while value 'MIP only' forces it on for mixed integer programming (MIP) models and value 'Always' forces it on for all types of models, including linear programming (LP) models, and MIP relaxations. The default value chooses automatically.

