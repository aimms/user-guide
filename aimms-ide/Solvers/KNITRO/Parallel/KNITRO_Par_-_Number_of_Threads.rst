.. _option-KNITRO-number_of_threads:


Number of Threads
=================



:Type:	Integer	
:Range:	{1..1000000}	
:Default:	1	



This option specifies the number of threads n to use for all parallel features other than parallel BLAS (which is controlled by the option **Number of BLAS Threads**).



This option can be used to let the four Knitro algorithms run in parallel, if the option **Algorithm** is set to 'Multi-algorithm'.



This option can also be used to let the multistart algorithm (as controlled by the option **Multistart**) run in parallel.



When the multistart procedure is run in parallel, Knitro will produce the same sequence of initial points and solves that you see when running multistart sequentially (though, perhaps, not in the same order). Therefore, as long as you run multistart to completion (setting the option **Multistart Termination Condition**  to 'Normal') and have the deterministic option **Multistart Deterministic**  switched on, you should visit the same initial points encountered when running multistart sequentially, and get the same final solution. By the default setting, the parallel multistart produces the same solution as the sequential multistart.



**Learn more about** 

*	:ref:`option-KNITRO-algorithm` 
*	:ref:`option-KNITRO-multistart`  
*	:ref:`option-KNITRO-multistart_deterministic`  
*	:ref:`option-KNITRO-multistart_termination_condition`  
*	:ref:`option-KNITRO-number_of_blas_threads` 



