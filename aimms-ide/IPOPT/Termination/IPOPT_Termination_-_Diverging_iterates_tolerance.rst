

.. _option-IPOPT-diverging_iterates_tolerance:


Diverging iterates tolerance
============================



:Type:	Floating point number	
:Range:	[1e-010,1e+019]	
:Default:	1e+019	



This option specifies the threshold for maximal value of primal iterates. If any component of the primal iterates exceeded this value (in absolute terms), the optimization is aborted with the exit message that the iterates seem to be diverging.

