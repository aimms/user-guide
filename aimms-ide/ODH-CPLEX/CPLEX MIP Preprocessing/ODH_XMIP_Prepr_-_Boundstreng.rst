.. _option-ODHCPLEX-boundstrength:


Boundstrength
=============



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Automatic	



Bound strengthening is used when solving MIPs. This process tightens the bounds on variables, perhaps to the point where the variable can be fixed and thus removed from consideration during branch-and-bound. This reduction is usually beneficial, but occasionally, due to its iterative nature, takes a long time. Possible values are:



*	Automatic
*	Off
*	On



