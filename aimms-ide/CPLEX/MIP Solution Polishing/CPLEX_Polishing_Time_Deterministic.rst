.. _option-CPLEX-polishing_time_deterministic:


Polishing Time Deterministic
============================



:Type:	Floating point number	
:Range:	[0,inf)	
:Default:	1e75	



This option sets the amount of time (expressed in deterministic ticks) to spend during a normal mixed integer optimization before CPLEX starts to polish a feasible solution. The default value is such that CPLEX does not start solution polishing by default.



CPLEX must have a feasible solution in order to start polishing. It must also have certain internal structures in place to support solution polishing. Consequently, when the criterion specified by this parameter is met, CPLEX begins solution polishing only after these starting conditions are also met. That is, there may be a delay between the moment when the criterion specified by this parameter is met and when solution polishing starts.



**Note** 

*	The option **Polishing Time** limits the amount of time spent in seconds (rather than deterministic ticks).




**Learn more about** 

*	:ref:`option-CPLEX-polishing_time`  
