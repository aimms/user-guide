.. _CPLEX_Barrier_-_Barrier_Start_Algori:


Barrier Start Algorithm
=======================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Default primal, dual pi is 0	



This option sets the algorithm to be used to compute the initial starting point for the Barrier Solver. The default starting point is satisfactory for most problems. Other starting points may provide better performance for certain problems, or provide better convergence properties for the barrier algorithm. Since the default starting point is tuned for primal problems, using other starting points may be worthwhile in conjunction with the option **Presolve Pass** . Possible values are:



*	Default primal, dual pi is 0
*	Default primal, estimate dual
*	Primal average, dual pi is 0
*	Primal average, estimate dual




**Learn more about** 

*	:ref:`CPLEX_Prepr_-_Presolve_Pass_D`  



