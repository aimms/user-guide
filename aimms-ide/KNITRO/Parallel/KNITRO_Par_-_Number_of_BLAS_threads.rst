.. _option-KNITRO-number_of_blas_threads:


Number of BLAS Threads
======================



:Type:	Integer	
:Range:	{1..1000000}	
:Default:	1	



This option specifies the number of threads to use for parallel BLAS. The BLAS function library can be used for basic vector and matrix computations, as controlled by the option **BLAS Option** .



**Note** 

*	Generally you should not use both parallel BLAS and a parallel linear solver (i.e., MKL PARDISO) as they may conflict with each other. If this option is set to a value greater than 1, one should set the option **Number of Linear System Threads**  to 1, and vice versa.




**Learn more about** 

*	:ref:`option-KNITRO-blas_option` 
*	:ref:`option-KNITRO-number_of_linear_system_threads` 
