.. _option-KNITRO-barrier_switch_objective:


Barrier Switch Objective
========================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Scalar weighting	



This option indicates which objective function to use when the barrier algorithms switch to a pure feasibility phase. Possible values are:



    *	Off
    *	Scalar weighting
    *	Diagonal weighting




With setting 'Off' no objective is used. Settings 'Scalar weighting' and 'Diagonal weighting' use a proximal point objective with scalar and diagonal weighting respectively.





This option has no effect on the Active Set and SQP algorithms.





**Learn more about** 

*	:ref:`option-KNITRO-algorithm` 
