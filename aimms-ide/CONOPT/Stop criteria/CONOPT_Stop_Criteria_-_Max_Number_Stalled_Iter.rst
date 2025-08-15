.. _CONOPT_Stop_Criteria_-_Max_Number_Stalled_Iter:

Maximal Number of Stalled Iterations
====================================



:Type:	Integer	
:Range:	{2..:ref:`Miscellaneous_Maxint` }	
:Default:	100	



This option sets the upper bound on the number of stalled iterations. CONOPT uses two definitions of a stalled iteration:



1: There is no change in the objective because something is bad, but the iteration is not degenerate. The iteration will be marked with 'F' in the column 'OK' in the iteration log. CONOPT will apply various heuristics such as changing the basis to make progress again.



2: When CONOPT approaches the optimum or when progress is slow, CONOPT will tighten the tolerances and the more accurate objective function value may become worse than the best seen so far. The iterations are counted as stalled as long as the current objective is worse than the best objective seen so far.



This option is used to prevent cycling for models with tolerance problems, usually very close to the optimal solution.



