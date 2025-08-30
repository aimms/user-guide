.. _option-KNITRO-number_of_multistart_threads:


Number of Multistart Threads
============================



:Type:	Integer	
:Range:	{0..1000000}	
:Default:	0		



This option specifies the number of threads to use for multistart. If the value is 0 then Knitro will choose the number of threads (currently sets it equal to **Number of Threads**). If set to a value n > 0 then n problems are solved in parallel.



When the multistart procedure is run in parallel, Knitro will produce the same sequence of initial points and solves that you see when running multistart sequentially (though, perhaps, not in the same order). Therefore, as long as you run multistart to completion (setting the option **Multistart Termination Condition**  to 'Normal') and have the deterministic option **Multistart Deterministic**  switched on, you should visit the same initial points encountered when running multistart sequentially, and get the same final solution.



**Learn more about** 

*	:ref:`option-KNITRO-multistart`  
*	:ref:`option-KNITRO-multistart_deterministic`  
*	:ref:`option-KNITRO-multistart_termination_condition`  
*	:ref:`option-KNITRO-number_of_threads`  
