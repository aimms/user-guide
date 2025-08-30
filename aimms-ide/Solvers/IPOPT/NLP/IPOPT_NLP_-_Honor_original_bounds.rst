

.. _option-IPOPT-honor_original_bounds:


Honor original bounds
=====================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Yes	



This option indicates whether final points should be projected into original bounds. IPOPT might relax the bounds during the optimization (see, e.g., the option **Factor for Initial Bounds Relaxation**). This option determines whether the final point should be projected back into the user-provide original bounds after the optimization. Possible values are:



    *	No (Leave final point unchanged)
    *	Yes (Project final point back into original bounds)




**Learn more about** 

*	:ref:`option-IPOPT-factor_for_initial_bounds_relaxation` 
