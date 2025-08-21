

.. _option-IPOPT-bound_multipliers_initialization_method:


Bound multipliers initialization method
=======================================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Constant	



This option defines how the iterates for the bound multipliers are initialized. Possible values are:



*	Constant
*	Mu-based




If 'Constant' is chosen then all bound multipliers are initialized to the value of the option **Initial Value for Bound Multipliers** . If 'Mu-based' is chosen then each value is initialized to the the value of the option **Barrier Parameter Initial Value**  divided by the corresponding slack variable. This latter option might be useful if the starting point is close to the optimal solution.





**Learn more about** 

*	:ref:`option-IPOPT-barrier_parameter_initial_value` 
*	:ref:`option-IPOPT-initial_value_for_bound_multipliers` 
