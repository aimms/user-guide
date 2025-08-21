.. _option-GUROBI-presolve_row_reduction:


Presolve Row Reduction
======================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Continuous models	



This option controls the presolve dependent row reduction, which eliminates linearly dependent constraints from the constraint matrix. The default setting applies the reduction to continuous models but not to MIP models. Setting 'Off' turns the reduction off for all models. Setting 'All models' turns it on for all models. Possible values are:



*	Continuous models
*	Off
*	All models



