.. _option-KNITRO-conjugate_gradient_memory_limit:


Conjugate Gradient Memory Limit
===============================



:Type:	Integer	
:Range:	{1..1000000}	
:Default:	10	



This option specifies the amount of nonzero elements per column of the Hessian of the Lagrangian which are retained when
computing the incomplete Cholesky preconditioner, as controlled by the option **Conjugate Gradient Preconditioner**.
Possible values are: 

    *n*:	At most *n* nonzero elements per column.


**Learn more about**

*	:ref:`option-KNITRO-conjugate_gradient_preconditioner`  
