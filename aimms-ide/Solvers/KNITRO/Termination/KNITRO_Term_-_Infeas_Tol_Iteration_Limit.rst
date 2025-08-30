.. _option-KNITRO-infeasibility_tolerance_iteration_limit:


Infeasibility Tolerance Iteration Limit
=======================================



:Type:	Integer	
:Range:	{1..1000000}	
:Default:	50	



This option can be used to control termination when there is little progress in getting feasible. The optimization process will terminate if the relative change in the feasibility error is less than the setting of the option **Infeasibility Tolerance** for :math:`n` consecutive infeasible iterations, where :math:`n` is the value of this option.



**Learn more about** 

*	:ref:`option-KNITRO-infeasibility_tolerance` 
