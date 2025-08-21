

.. _Limits_-_Unbounded_Step_Size:
.. _option-MINOS-unbounded_step_size:


Unbounded Step Size
===================



:Type:	Floating point number	
:Range:	[1e-15,1e20]	
:Default:	1e10	



This option is intended to detect unboundedness in nonlinear problems. 
(It may not achieve that purpose!). 
During a line search, a function F is evaluated at points of the forms x + ap, where x and p are fixed and a varies. 
If a exceeds the value of this option (or if :math:`|F|` exceeds the value of the option **Unbounded Objective Value** ), 
iterations are terminated with the exit message "problem is unbounded" (or "badly scaled").



Unboundedness in x is best avoided by placing finite upper and lower bounds on the variables.



**Learn more about** 

*	:ref:`option-MINOS-unbounded_objective_value`  



