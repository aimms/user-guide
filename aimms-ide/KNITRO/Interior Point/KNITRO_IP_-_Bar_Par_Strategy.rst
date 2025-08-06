.. _KNITRO_IP_-_Bar_Par_Strategy:


Barrier Parameter Strategy
==========================



**Type** :	Selection	

**Range** :	The settings listed below	

**Default** :	Automatic	



This option determines which strategy Knitro should use for modifying the barrier parameter in the interior point code. Possible values are:



*	Automatic
*	Monotone
*	Adaptive
*	Probing
*	Mehrotra with safeguards
*	Mehrotra without safeguards
*	Quality




With setting 'Monotone' Knitro will monotonically decrease the barrier parameter. With setting 'Adaptive' Knitro uses an adaptive rule based on the complementarity gap to determine the value of the barrier parameter at every iteration. With 'Probing' Knitro uses a probing (affine-scaling) step to dynamically determine the barrier parameter value at each iteration. For the Mehrotra settings Knitro uses a Mehrotra predictor-corrector type rule to determine the barrier parameter with or without safeguards on the corrector step. With setting 'Quality' Knitro minimizes a quality function at each iteration to determine the barrier parameter.





All strategies are available for the Interior-Direct algorithm but for the Interior-CG algorithm only the first three strategies are available.The two Mehrotra strategies are typically recommended for linear programs or convex quadratic programs. Many problems benefit from a non-default setting of this option and it is recommended to experiment with all settings. In particular we recommend trying strategy 'Quality' when using the Interior-Direct algorithm.





This option has no effect on the Active Set and SQP algorithms.





**Learn more about** 

*	:ref:`KNITRO_General_-_Algorithm` 



