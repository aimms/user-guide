

.. _IPOPT_Linear_solver_-_Linear_system_scaling_method:


Linear system scaling method
============================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	None	



This option determines the method used to compute symmetric scaling factors for the augmented system (see also the option **Linear System Scaling** ). This scaling is independent of the NLP problem scaling. By default, MC19 is only used if MA27 or MA57 is selected as linear solver as controlled by the option **Linear Solver Selection** . Possible values are:



*	None
*	MC19




**Note** 

*	This option is only used if the user has provided a DLL with HSL subroutines. 




**Learn more about** 

*	:ref:`IPOPT_Linear_solver_-_Linear_solver_selection` 
*	:ref:`IPOPT_Linear_solver_-_Linear_system_scaling` 
