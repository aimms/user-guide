.. _GUROBI_MIP_-_MIP_Focus:


MIP Focus
=========



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Balanced	



The option controls the focus of the MIP solver. The default value tries to strike a balance between finding good feasible solutions and proving optimality. A value of 'Feasibility' shifts the focus towards finding feasible solutions. A value of 'Optimality' shifts the focus towards proving optimality. A value of 'Best bound' focuses almost entirely on moving the best objective bound. Possible values are:



*	Balanced
*	Feasibility
*	Optimality
*	Best bound



