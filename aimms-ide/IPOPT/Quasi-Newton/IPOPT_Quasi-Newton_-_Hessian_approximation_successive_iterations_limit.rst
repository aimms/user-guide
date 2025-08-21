

.. _option-IPOPT-hessian_approximation_successive_iterations_limit:


Hessian approximation successive iterations limit
=================================================



:Type:	Integer	
:Range:	{1..2147483647}	
:Default:	2	



This option specifies the threshold for successive iterations where update is skipped. If the update is skipped more than this number of successive iterations, the quasi-Newton approximation is reset.



**Note** 

*	This option is only used if the option **Method for Hessian Computation**  has been set to 'Quasi-Newton', or to 'Automatic' and no Hessian is available in AIMMS. 




**Learn more about** 

*	:ref:`option-IPOPT-method_for_hessian_computation` 
