

.. _Advanced_-_Function_Precision:
.. _MINOS_Advanced_-_Function_Precision:


Function Precision
==================



:Type:	Floating point number	
:Range:	[1e-15,1] + {na}	
:Default:	na	



The (relative) function precision e is intended to be a measure of the relative accuracy with which the nonlinear functions can be computed. For example, if F(x) is computed as 1000.56789 for some relevant x and if the first 6 significant digits are known to be correct, the appropriate value for e would be 1.0e-6.



Ideally the functions F(x) or f'(x) should have a magnitude of order 1. If all functions are substantially less than 1 in magnitude, e should be the absolute precision. For example, if F(x) = 1.23456789e-4 at some point and if the first 6 significant digits are known to be correct, the appropriate value for e would be 1.0e-10.



The default value of this option is appropriate for simple analytic functions.



In some cases the function values will be the result of an extensive computation, possibly involving an iterative procedure that can provide rather few digits of precision at reasonable cost. Specifying an appropriate function precision may lead to savings, by allowing the linesearch procedure to terminate when the difference between function values along the search direction becomes as small as the absolute error in the values.



The default value of this option depends on the relative precision of the computer being used. On most computers the default equals 3.0e-13.



