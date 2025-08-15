

.. _IPOPT_Linear_solver_-_Linear_system_scaling:


Linear system scaling
=====================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Yes	



This option indicates that linear scaling is only done if it seems required. This option is only important if a linear scaling method (e.g., MC19) is used as determined by the option **Linear System Scaling Method** . If switched off, then the scaling factors are computed for every linear system from the start. This can be quite expensive. Setting 'Yes' means that the algorithm will start the scaling method only when the solutions to the linear system seem not good, and then use it until the end. Possible values are:



*	No
*	Yes




**Learn more about** 

*	:ref:`IPOPT_Linear_solver_-_Linear_system_scaling_method` 
