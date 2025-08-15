

.. _IPOPT_NLP_-_Check_derivatives_for_invalid_numbers:


Check derivatives for invalid numbers
=====================================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	No	



This option indicates whether it is desired to check for invalid numbers (na, inf) in the derivative matrices. Activating this option will cause an error if an invalid number is detected in the constraint Jacobians or the Lagrangian Hessian. If this is not activated, the test is skipped, and the algorithm might proceed with invalid numbers and fail. If the test is activated and an invalid number is detected, the matrix is written to output if option **Output Verbosity Level**  is set to a large value; so beware of large output! 



Possible values are:



*	No
*	Yes




**Learn more about** 

*	:ref:`IPOPT_Output_-_Output_verbosity_level` 
