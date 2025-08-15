.. _GUROBI_Barrier_-_Barrier_Homogeneous_Aalgorithm:


Barrier Homogeneous Algorithm
=============================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Automatic



This option determines whether to use the homogeneous barrier algorithm. At the default setting ('Automatic'), it is only used when barrier solves a node relaxation for a MIP model. The homogeneous algorithm is useful for recognizing infeasibility or unboundedness. It is a bit slower than the default algorithm. Possible values are:



*	Automatic
*	Off
*	On
