.. _option-KNITRO-barrier_slack_bound_push:


Barrier Slack Bound Push
========================



:Type:	Floating point number	
:Range:	[0,1e20]	
:Default:	0.1	



This option specifies the amount by which the barrier slack variables are initially pushed inside the bounds. A smaller value may be preferable when warm-starting from a point close to the solution.



This option has no effect on the Active Set and SQP algorithms.



**Learn more about** 

*	:ref:`option-KNITRO-algorithm` 
