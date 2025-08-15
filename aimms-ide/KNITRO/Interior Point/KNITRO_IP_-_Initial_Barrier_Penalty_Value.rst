.. _KNITRO_IP_-_Initial_Barrier_Penalty_Value:


Initial Barrier Penalty Value MPEC
==================================



**Type**:	Floating point number	

**Range**:	[0,1e20]	

**Default**:	0



This option specifies the initial value for the MPEC penalty parameter used when solving problems with complementarity constraints using the barrier algorithms. If this value is equal to 0, then Knitro uses an internal formula to initialize the MPEC penalty parameter.

