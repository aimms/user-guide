.. _KNITRO_General_-_Unbound_**Range**:


Unboundedness Range
===================



**Type**:	Floating point number	

**Range**:	[0,1e20]	

**Default**:	1e20	



This option determines the allowable range of values for the objective function for determining unboundedness. If the magnitude of the objective function is greater than the value of this option and the iterate is feasible, then the problem is determined to be unbounded.



