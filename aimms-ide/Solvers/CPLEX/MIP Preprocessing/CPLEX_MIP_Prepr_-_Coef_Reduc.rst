.. _option-CPLEX-coefficient_reduction:


Coefficient Reduction
=====================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Automatic	



Coefficient reduction is a technique used when presolving mixed integer programs. The benefit of coefficient reduction is to improve the objective value of the initial (and subsequent) linear programming relaxations solved during branch-and-bound by reducing the number of non-integral vertices. However, the linear programs generated at each node may become more difficult to solve. There is a resulting tradeoff between reducing the number of nodes in the branch-and-bound tree and the time to solve each node via a linear programming algorithm. Full coefficient reduction reduces all possible coefficients, while integer coefficient reduction will only reduce coefficients to integer values. Possible values are:



    *	Automatic
    *	None
    *	Only integral coefficients
    *	All possible coefficients
    *	Aggressively with tilting




By default, CPLEX decides. Setting 'None' turns off coefficient reduction during preprocessing.





Setting 'Only integral coefficients' applies limited coefficient reduction to achieve only integral coefficients. 





Setting 'All possible coefficients' applies coefficient reduction somewhat more aggressively, reducing all coefficients that can be reduced.





Setting 'Aggressively with tilting', the most aggressive setting of this option, applies a technique known as tilting. Tilting can cut off additional fractional solutions in some models. Cutting off these fractional solutions potentially yields more progress in both the best node and best integer solution in those particular models.

