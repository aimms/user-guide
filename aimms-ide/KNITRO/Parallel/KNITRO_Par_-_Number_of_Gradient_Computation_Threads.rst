.. _option-KNITRO-number_of_gradient_computation_threads:


Number of Gradient Computation Threads
======================================

:Type:	Integer	
:Range:	{0..1000000}	
:Default:	0	



This option specifies the number of threads to use when computing finite-difference gradients by Knitro. The value of 0 lets Knitro choose the number of threads.



This option is only used if the option **Gradient Computation Method**  is set to a non-default value.



**Learn more about** 

*	:ref:`option-KNITRO-gradient_computation_method` 
