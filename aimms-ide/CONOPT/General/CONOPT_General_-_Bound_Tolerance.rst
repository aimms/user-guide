.. _option-CONOPT-bound_tolerance:

Bound Tolerance
===============



:Type:	Floating point number	
:Range:	[3e-13,1e-5]
:Default:	1e-7	



This option defines the bound filter tolerance for solution values close to a bound. A variable is considered to be at a bound if its distance from the bound is less than BT * Max(1,ABS(Bound)), where BT denotes the value of this option. The tolerance is used to build the initial bases and is used to flag variables during output.



