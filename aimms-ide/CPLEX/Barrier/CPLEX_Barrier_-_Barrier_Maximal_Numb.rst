.. _CPLEX_Barrier_-_Barrier_Maximal_Numb:


Barrier Maximal Number of Corrections
=====================================



**Type**:	Integer	

**Range**:	{-1 .. 2147483647}	

**Default**:	-1	



This option is used to set the maximum number of centering corrections done on each iteration. By default, the Barrier Solver automatically computes an estimate value for this option (the computed value can be observed by setting the option **Barrier Display**  to "Diagnostics"). When using the default barrier algorithm, if the computed value is 0, setting the value to an explicit value greater than 0 may improve the numerical performance of the algorithm at the expense of computation time. Possible values are:



-1:	Automatically determined	

0:	No corrections	

n:	n corrections	



**Learn more about** 

*	:ref:`CPLEX_Logging_-_Barrier_Display` 



