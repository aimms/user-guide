.. _KNITRO_IP_-_Conjugate_Gradient_Memory_Limit:


Conjugate Gradient Memory Limit
===============================



:Type:	Integer	
:Range:	{1..1000000}	
:Default:	10	



This option specifies the amount of nonzero elements per column of the Hessian of the Lagrangian which are retained when computing the incomplete Cholesky preconditioner, as controlled by the option **Conjugate Gradient Preconditioner** . Possible values are: 



n:	At most n nonzero elements per column.



**Learn more about** 

*	:ref:`KNITRO_IP_-_Conjugate_Gradient_Preconditio`  
