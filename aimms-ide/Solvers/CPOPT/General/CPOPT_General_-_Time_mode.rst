.. _option-CPOPT-time_mode:


Time mode
=========



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Elapsed time	



This option defines how time is measured in CP Optimizer. CP Optimizer uses time for both display purposes and for limiting the search via the general solvers option **Time Limit** . Note that when multiple processors are available and the number of workers is greater than one, then the CPU time can be greater than the elapsed time by a factor up to the number of workers.



Possible values are:



    *	CPU time
    *	Elapsed time




**Learn more about** 

*	:ref:`option-CPOPT-number_of_workers` 
*	:ref:`option-AIMMS-time_limit`  
