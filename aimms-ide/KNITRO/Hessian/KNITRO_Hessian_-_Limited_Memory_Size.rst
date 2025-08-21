.. _option-KNITRO-limited_memory_size:


Limited Memory Size
===================



:Type:	Integer	
:Range:	{1..100}	
:Default:	10	



This option specifies the number of limited memory pairs stored when approximating the Hessian using the limited-memory quasi-Newton BFGS option. This option is only used if the option **Hessian Computation Method**  is set to 'Limited-memory BFGS Hessian'.



Larger values may give a more accurate, but more expensive, Hessian approximation. Smaller values may give a less accurate, but faster, Hessian approximation. When using the limited memory BFGS approach it is recommended to experiment with different values of this option.



**Learn more about** 

*	:ref:`option-KNITRO-hessian_computation_method` 
