.. _KNITRO_MIP_-_MIP_Rounding:


MIP Rounding
============



**Type**:	Selection	

**Range**:	The settings listed below	

**Default**:	Automatic	



This option specifies the MIP rounding rule to apply. Possible values are:



*	Automatic
*	None
*	Fast heuristic
*	Solve sometimes
*	Solve always




Setting 'None' implies no rounding if a node is infeasible. Setting 'Fast heuristic' means round using a fast heuristic only. Setting 'Solve sometimes' means do round and solve a subproblem if it is likely to succeed. Setting 'Solve always' implies always round and solve a subproblem.

