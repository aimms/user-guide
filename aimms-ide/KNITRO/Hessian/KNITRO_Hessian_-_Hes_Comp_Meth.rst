.. _KNITRO_Hessian_-_Hes_Comp_Meth:


Hessian Computation Method
==========================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	AIMMS computes	



This option specifies how to compute the (approximate) Hessian of the Lagrangian. By default AIMMS will compute the Hessian. Only in some rare situations the setting of this option should be changed. Possible values are:



*	AIMMS computes
*	Quasi-Newton BFGS Hessian
*	Quasi-Newton SR1 Hessian
*	Hessian-vector products
*	Limited-memory BFGS Hessian




With setting 'Hessian-vector products' Knitro will use a finite difference method to calculate the vector products based on the exact gradients. In terms of robustness it is comparable to the 'AIMMS computes' setting and typically not too much slower in terms of time if gradient evaluations are not the dominant cost. The setting 'Hessian-vector products' cannot be used for the Interior-Direct algorithm. With the setting 'Limited-memory BFGS Hessian' Knitro tries to approximate the Hessian matrix using a limited amount of storage. This setting should only be used for very large problems where memory is a bottleneck.





**Learn more about** 

*	:ref:`KNITRO_General_-_Algorithm`  
