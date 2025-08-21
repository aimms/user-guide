.. _option-GUROBI-multi_objective_presolve:


Multi Objective Presolve
========================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Automatic	



This option controls the initial presolve level used for multi-objective models. Possible values are:



*	Automatic
*	Off
*	Conservative
*	Aggressive




The default value 'Automatic' usually applies presolve conservatively. Aggressive presolve may increase the chance of the objective values being slightly different than those for other options.

