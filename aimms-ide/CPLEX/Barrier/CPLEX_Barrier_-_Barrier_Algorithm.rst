.. _option-CPLEX-barrier_algorithm:


Barrier Algorithm
=================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Default standard algorithm	



The default barrier algorithm is almost always fastest. However, on problems that are primal or dual infeasible, the default algorithm may not work as well as alternatives. The two alternative algorithms may eliminate numerical difficulties related to infeasibility, but will generally be slower. Possible values are:



*	Default standard algorithm
*	Infeasibility-estimate start
*	Infeasibility-constant start
*	Standard barrier



