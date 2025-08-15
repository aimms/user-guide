.. _KNITRO_General_-_Linear_Solver_Ordering:


Linear Solver Ordering
======================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Automatic	



Ths option sets the ordering method used by the **Linear Solver.** Possible values are:



*	Automatic
*	Best
*	AMD
*	METIS




With the default setting 'Automatic', let Knitro determine which ordering to use. 





With the setting 'Best', Knitro tries both 'AMD' and 'METIS' and chooses the best ordering.





With the setting 'AMD', use AMD ordering (minimum degree for 'MKL PARDISO').





With the setting 'METIS', use METIS ordering.





**Learn more about** 

*	:ref:`KNITRO_General_-_Linear_Solver` 
