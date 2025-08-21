.. _option-KNITRO-qp_algorithm:


QP Algorithm
============



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Automatic	



This option indicates which algorithm to use to solve quadratic programming (QP) subproblems when using the Active Set or SQP algorithms, as determined by the option **Algorithm** . At the default setting Knitro will automatically try to choose the best algorithm based on the problem characteristics. Possible values are:



*	Automatic
*	Interior-Direct
*	Interior-CG
*	Active-Set




**Note** 

*	This option has no effect on the Interior-Direct and Interior-CG algorithms.




**Learn more about** 

*	:ref:`option-KNITRO-algorithm` 
