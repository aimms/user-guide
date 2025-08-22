.. _option-CPLEX-barrier_progress_solution:


Barrier Progress Solution
=========================



:Type:	Integer	
:Range:	{0 .. 2100000000}	
:Default:	0	



This option controls the progress reports during the solution process if the barrier solver is used by CPLEX. If the Progress Window is open, it will display information about the number of (barrier) iterations, the current status, the best value found, etc. Possible values are: 



0:	Do not report progress	

n:	Report progress after each n barrier iterations	



**Note** 

*	This option overrules the setting of the general solvers option **Progress Solution**  in case the barrier solver is used, and CPLEX is not in the Barrier crossover phase.




**Learn more about** 

*	:ref:`option-AIMMS-progress_solution` 
