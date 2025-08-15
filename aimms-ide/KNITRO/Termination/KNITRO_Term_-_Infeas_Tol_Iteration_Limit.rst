.. _KNITRO_Term_-_Infeas_Tol_Iteration_Limit:


Infeasibility Tolerance Iteration Limit
=======================================



**Type**:	Integer	

**Range**:	{1..1000000}	

**Default**:	50	



This option can be used to control termination when there is little progress in getting feasible. The optimization process will terminate if the relative change in the feasibility error is less than the setting of the option**Infeasibility Tolerance**  for n consecutive infeasible iterations, where n is the value of this option.



**Learn more about** 

*	:ref:`KNITRO_Tol_-_Infeasibility_Tolerance` 
