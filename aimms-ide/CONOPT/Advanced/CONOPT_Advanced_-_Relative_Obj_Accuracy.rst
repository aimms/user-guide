.. _option-CONOPT-relative_objective_accuracy:


Relative Objective Accuracy
===========================



:Type:	Floating point number	
:Range:	[3e-14,1e-6]
:Default:	3e-13	



CONOPT assumes that the reduced objective function can be computed to an accuracy of the value of this option* max(1,|fobj|), where fobj is the value of the current objective function. The value is used in tests for "Slow Progress".



**Learn more about** 

*	:ref:`option-CONOPT-limit_for_slow_progress`  



