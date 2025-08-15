

.. _Options_Matrix_Generation_-_Open_Bound:


Open Bound Tolerance
====================



:Type:	Floating point number	
:Range:	[0.0, 0.1]	
:Default:	1.0e-6	



This option is used to specify open bounds for solvers. In an AIMMS model a variable is allowed to have an open bound. For example:



``VARIABLE:`` 

``identifier : x`` 

``range : ( 0.0, 1.0 ] ;`` 



The left bound of x is open and the right bound is closed. Solvers can in general only handle closed bounds. AIMMS will add/substract the value of this option to an open bound and pass the result to the solver as a closed bound.





