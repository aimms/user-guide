.. _KNITRO_IP_-_Barrier_Corrector_Steps_Limit:


Barrier Corrector Steps Limit
=============================



:Type:	Integer	
:Range:	{-1..1000000}	
:Default:	-1	



This option specifies the maximum number of corrector steps allowed for primal-dual steps. If the value is positive and the algorithm used is Interior/Direct, then Knitro may add at most n corrector steps, where n is the value of this option, to the primal-dual step to try to stay closer to the central path. This may speedup convergence on some models (although it may make the cost per iteration a little more expensive).



If the value equals -1, Knitro automatically determines the maximum number of corrector steps to apply.



This option has no effect on the Active Set and SQP algorithms.



**Learn more about** 

*	:ref:`KNITRO_General_-_Algorithm` 



