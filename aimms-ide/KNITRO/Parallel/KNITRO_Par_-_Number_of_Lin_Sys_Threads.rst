.. _KNITRO_Par_-_Number_of_Lin_Sys_Threads:


Number of Linear System Threads
===============================



**Type**:	Integer	

**Range**:	{1..1000000}	

**Default**:	1		



This option specifies the number of threads to use for linear system solve operations when using the MKL PARDISO linear solver.



This option only has effect if the option **Linear Solver**  is set to 'MKL PARDISO'.



**Note** 

*	Generally you should not use both parallel BLAS and a parallel linear solver (i.e., MKL PARDISO) as they may conflict with each other. If this option is set to a value greater than 1, one should set the option **Number of BLAS Threads**  to 1, and vice versa.




**Learn more about** 

*	:ref:`KNITRO_General_-_Linear_Solver`  
*	:ref:`KNITRO_Par_-_Number_of_BLAS_threads` 
