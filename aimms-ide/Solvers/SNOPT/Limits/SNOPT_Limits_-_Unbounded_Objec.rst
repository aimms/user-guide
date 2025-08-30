.. _option-SNOPT-unbounded_objective_value:


Unbounded Objective Value
=========================



:Type:	Floating point number	
:Range:	[0,1e20]	
:Default:	1e20	



This option is intended to detect unboundedness in nonlinear problems. (It may not achieve that purpose!). During a line search, a function f is evaluated at points of the forms x + ap, where x and p are fixed and a varies. If | f | exceeds the value of this option (or if a exceeds the value of the option **Unbounded Step Size**), iterations are terminated with the exit message "problem is unbounded" (or "badly scaled").



If singularities are present, unboundedness in f(x) may be manifested by a floating-point overflow (during the evaluation of f(x + ap)), before the test for ``| f |``  against the unbounded objective value can be made.



Unboundedness in x is best avoided by placing finite upper and lower bounds on the variables.



**Learn more about** 

*	:ref:`option-SNOPT-unbounded_step_size`  



