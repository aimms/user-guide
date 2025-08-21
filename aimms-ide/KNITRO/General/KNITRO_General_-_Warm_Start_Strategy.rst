.. _option-KNITRO-warm_start_strategy:


Warm Start Strategy
===================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	On	



This option specifies whether or not to invoke a warm-start strategy. Possible values are:



*	Off
*	On




A warm-start strategy may be beneficial when an initial point close to the solution can be provided. For example, this may occur when solving a sequence of closely related problems, and the solution from one problem can


be used to initialize (or warm-start) the next problem in the sequence. The Knitro warm-start strategy will use this information to tune the algorithms to try to converge more quickly in this case. If the initial point is not


sufficiently close to the solution, or is too infeasible, the warm-start strategy may not be helpful.





This option is currently only used for the Knitro barrier/interior-point algorithms. In this case it may also be useful to experiment with different (smaller than default) values for the initial barrier option **Initial Barrier Parameter Value** . In general, the closer the initial point is to the solution, the smaller this value should be (Knitro will try by default to initialize this to a good value when applying a warm-start strategy).





**Learn more about** 

*	:ref:`option-KNITRO-algorithm` 
*	:ref:`option-KNITRO-initial_barrier_parameter_value` 
