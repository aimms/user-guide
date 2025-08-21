.. _option-CPLEX-adjust_miqp:


Adjust MIQP
===========



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Yes	



This option determines whether CPLEX will attempt to adjust a MIQP formulation, in which all the variables appearing in the quadratic term are binary. When this option is active (the default), adjustments will be made to the elements of a quadratic matrix that is not nominally positive semi-definite (as required for all QP formulations), to make it positive semi-definite, and will also attempt to tighten an already positive semi-definite matrix for better numerical behavior. Possible values are:



*	No
*	Yes






