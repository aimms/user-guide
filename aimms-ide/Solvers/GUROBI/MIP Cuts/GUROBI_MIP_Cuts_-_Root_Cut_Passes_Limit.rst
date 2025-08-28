.. _option-GUROBI-root_cut_passes_limit:


Root Cut Passes Limit
=====================



:Type:	Integer	
:Range:	{-1 .. 2000000000}	
:Default:	-1	



This option controls the maximum number of cutting plane passes performed during root cut generation. At the default setting of -1, Gurobi chooses the number of cut passes automatically.



You should experiment with different values of this option if you notice the MIP solver spending significant time on root cut passes that have little impact on the objective bound.

