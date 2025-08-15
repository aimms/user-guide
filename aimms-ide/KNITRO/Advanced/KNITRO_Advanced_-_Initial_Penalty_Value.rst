.. _KNITRO_Advanced_-_Initial_Penalty_Value:


Initial Penalty Value
=====================



**Type**:	Floating point number	

**Range**:	[0,1e20]	

**Default**:	10	



This option specifies the initial penalty parameter used in the Knitro merit functions. The Knitro merit functions are used to balance improvements in the objective function versus improvements in feasibility. A larger initial penalty value places more weight initially on feasibility in the merit function.

