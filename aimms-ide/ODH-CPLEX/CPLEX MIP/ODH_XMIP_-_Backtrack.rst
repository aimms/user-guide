.. _ODH-CPLEX_XMIP_-_Backtrack:


Backtrack
=========



:Type:	Floating point number	
:Range:	[0, 1]	
:Default:	0.9999	



This option controls how often backtracking is done during the branching process. At each node, CPLEX compares the objective function value or estimated integer objective value to these values at parent nodes; this option dictates how much relative degradation is tolerated before backtracking. Low values tend to increase the amount of backtracking, which makes the search process more of a pure best-bound search. Higher values, close to 1.0, tend to decrease backtracking, making the search more of a pure depth-first search. While the default value is good for many models, increased backtracking (lower values) often pays off on models that have expensive subproblems. 



