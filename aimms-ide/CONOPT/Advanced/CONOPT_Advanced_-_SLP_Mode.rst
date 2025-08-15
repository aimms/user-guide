.. _CONOPT_Advanced_-_SLP_Mode:

SLP Mode
========



:Type:	Selection	
:Range:	The settings listed below	
:Default:	On	



When the model continues to appear linear, CONOPT will often take many small steps, each determined by a new variable reaching a bound. Although the line searches are fast in linear mode, each require one or more evaluations of the constraints, and the overall cost may become high. In order to avoid the many constraint evaluations, CONOPT may use a Sequential Linear Programming (SLP) technique to find a search direction that anticipates the bounds on all variables, and at the same time gives a larger expected change in objective. The search direction from the SLP procedure is used in an ordinary GRG-type line search in which the solution is made feasible at each step. The SLP procedure is only used to generate good directions; the usual feasibility preserving steps in CONOPT are maintained. Possibly values are:



*	Off
*	On



