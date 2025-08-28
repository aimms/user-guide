.. _option-KNITRO-number_of_linear_system_threads:


Number of Linear System Threads
===============================



:Type:	Integer	
:Range:	{1..1000000}	
:Default:	1		



This option specifies the number of threads to use for linear system solve operations when using the MKL PARDISO linear solver.



This option only has effect if the option **Linear Solver**  is set to 'MKL PARDISO'.



**Note** 

*	Generally you should not use both parallel BLAS and a parallel linear solver (i.e., MKL PARDISO) as they may conflict with each other. If this option is set to a value greater than 1, one should set the option **Number of BLAS Threads**  to 1, and vice versa.




**Learn more about** 

*	:ref:`option-KNITRO-linear_solver`  
*	:ref:`option-KNITRO-number_of_blas_threads` 
