.. _option-MINOS-unbounded_objective_value:


Unbounded Objective Value
=========================



:Type:	Floating point number	
:Range:	[1e-15,1e20]	
:Default:	1e20	



This option is intended to detect unboundedness in nonlinear problems. 
(It may not achieve that purpose!). 
During a line search a function :math:`F` is evaluated at points of the forms :math:`x + \alpha p`, where :math:`x` and :math:`p` are fixed and :math:`\alpha` varies. 
If :math:`|F|` exceeds the value of this option (or if :math:`\alpha` exceeds the value of the option **Unbounded Step Size**), 
iterations are terminated with the exit message "problem is unbounded" (or "badly scaled").

If singularities are present, unboundedness in :math:`F(x)` may be manifested by a floating-point overflow (during the evaluation of :math:`F(x + \alpha p)`),
before the test against the unbounded objective value can be made.

Unboundedness in :math:`x` is best avoided by placing finite upper and lower bounds on the variables.



**Learn more about** 

*	:ref:`option-MINOS-unbounded_step_size`  



