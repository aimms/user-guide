

.. _Advanced_-_Linesearch_Toleranc:
.. _option-MINOS-linesearch_tolerance:


Linesearch Tolerance
====================



:Type:	Floating point number	
:Range:	[0,1]	
:Default:	0.1	



For nonlinear problems, this option controls the accuracy with which an optimum of the merit function will be located along the direction of search each iteration. The default value of 0.1 requests a moderately accurate search. It should be satisfactory for many problems.



If the nonlinear functions are cheap to evaluate, a more accurate search may be appropriate; try 0.01 or 0.001. The number of major iterations should decrease, and this will reduce the total run time if there are many linear or nonlinear constraints.



If the nonlinear functions are expensive to evaluate, a less accurate search may be appropriate. If all gradients are known, try 0.5 or perhaps 0.9. (The number of iterations will probably increase, but the total number of function evaluations may decrease enough to compensate.)

