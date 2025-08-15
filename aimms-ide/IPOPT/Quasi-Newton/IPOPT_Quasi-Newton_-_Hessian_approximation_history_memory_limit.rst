

.. _IPOPT_Quasi-Newton_-_Hessian_approximation_history_memory_limit:


Hessian approximation history memory limit
==========================================



:Type:	Integer	
:Range:	{0..2147483647}	
:Default:	6	



This option specifies the maximum size of the history for the limited quasi-Newton Hessian approximation. It determines the number of most recent iterations that are taken into account for the limited-memory quasi-Newton approximation.



**Note** 

*	This option is only used if the option **Method for Hessian Computation**  has been set to 'Quasi-Newton', or to 'Automatic' and no Hessian is available in AIMMS. 




**Learn more about** 

*	:ref:`IPOPT_Quasi-Newton_-_Method_for_Hessian_computation` 
