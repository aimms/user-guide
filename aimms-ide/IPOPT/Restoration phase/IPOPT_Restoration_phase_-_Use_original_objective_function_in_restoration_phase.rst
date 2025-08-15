

.. _IPOPT_Restoration_phase_-_Use_original_objective_function_in_restoration_phase:


Use original objective function in restoration phase
====================================================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Yes	



This option determines if the original objective function should be evaluated at restoration phase trial points. Setting this option to 'Yes' makes the restoration phase algorithm evaluate the objective function of the original problem at every trial point encountered during the restoration phase, even if this value is not required. In this way, it is guaranteed that the original objective function can be evaluated without error at all accepted iterates; otherwise the algorithm might fail at a point where the restoration phase accepts an iterate that is good for the restoration phase problem, but not the original problem. On the other hand, if the evaluation of the original objective is expensive, this might be costly. Possible values are:



*	No
*	Yes



