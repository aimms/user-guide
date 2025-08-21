.. _option-CPLEX-clock_type:


Clock Type
==========



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Wall clock time	



This option decides how computation times are measured for both reporting performance and terminating optimization when a time limit has been set. Small variations in measured time on identical runs may be expected on any computer system with any setting of this option. Possible values are:



*	Automatic
*	CPU time
*	Wall clock time




The setting 'Automatic' allows CPLEX to choose wall clock time when other options invoke parallel optimization and to choose CPU time when other options enforce sequential (not parallel) optimization.





**Learn more about** 

*	 :ref:`option-CPLEX-global_thread_limit` 



