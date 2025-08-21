

.. _RadiusofConvergence:
.. _option-MINOS-radius_of_convergence:


Radius of Convergence
=====================



:Type:	Floating point number	
:Range:	[1e-7,1]	
:Default:	0.01	



This option determines when the penalty parameter r will be reduced (if initialized to a positive value). Both the nonlinear constraint violation (see option **Row Tolerance** ) and the relative change in consecutive Lagrange multipler estimates must be less than the value of this option at the start of a major iteration before r is reduced or set to zero. Once r is zero, the sequence of major iterations should converge quadratically to an optimum.



**Learn more about** 

*	:ref:`option-MINOS-penalty_parameter`  
*	:ref:`option-MINOS-row_tolerance`  
