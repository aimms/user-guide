.. _option-CPLEX-perturbation_indicator:


Perturbation Indicator
======================



:Type:	Selection	
:Range:	One of the settings listed below	
:Default:	When needed	



Setting this option to 'Always' will cause all problems to be automatically perturbed as optimization begins. The default
setting allows CPLEX to determine dynamically, during solution, whether progress is slow enough to merit a perturbation.
The situations in which a non-default setting helps will be rare and restricted to problems that exhibit extreme degeneracy.
Possible values are:

    *	When needed
    *	Always

