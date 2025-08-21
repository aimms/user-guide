.. _option-Baron-relative_termination_tolerance:


Relative termination tolerance
==============================



:Type:	Floating point number	
:Range:	[1e-9,1e51]	
:Default:	1e-6	



BARON terminates if :math:`L > ¥` or :math:`U - L <= e | L |`, 
where :math:`L` and :math:`U` are the lower and upper bounds to the optimization problem at the current iteration, and 
:math:`e` denotes the value of this option.



**Learn more about** 

*	:ref:`option-Baron-absolute_termination_tolerance` 



