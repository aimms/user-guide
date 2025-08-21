.. _option-KNITRO-multi_algorithm_termination:


Multi Algorithm Termination
===========================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Optimal	



This option defines the termination condition for the multi-algorithm procedure. Possible values are:



*	All (Terminate after all algorithms have completed)
*	Optimal (Terminate at first locally optimal solution)
*	Feasible (Terminate at first feasible solution estimate)
*	Any (Terminate at first solution estimate of any type)




This option is only active if the option **Algorithm**  is set to 'Multi-algorithm'.





**Learn more about** 

*	:ref:`option-KNITRO-algorithm` 
