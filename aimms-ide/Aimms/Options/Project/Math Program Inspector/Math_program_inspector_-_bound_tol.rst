

.. _option-AIMMS-mpi_bound_tolerance:


MPI Bound Tolerance
===================



:Type:	Selection	
:Range:	[0,1]	
:Default:	0.0001	



The Math Program Inspector reports several statistics on the math program under investigation. More specific, the 'bound tolerance' is used to determine whether or not

*	a constraint is binding,
*	a variable is at one of its bounds, and
*	the math program is primal degenerated




**Note** 

*	For badly scaled models, a discrepancy between the results from the solver and the statistics reported by the Math Program Inspector might occur for some values of the 'bound tolerance' (and/or 'feasibility tolerance'). 
*	This tolerance is not used for calculating the maximum and total bound violation on the Variable Statistics tab.




**Learn more about** 

*	:ref:`aimmshelp26-Math_Program_Inspector`  






