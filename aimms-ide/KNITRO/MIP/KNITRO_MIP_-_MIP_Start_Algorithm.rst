.. _KNITRO_MIP_-_MIP_Start_Algorithm:


MIP Start Algorithm
===================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Automatic	



This option specifies which algorithm to use for the root node solve in the branch and bound procedure. At the default setting Knitro will automatically try to choose the best algorithm based on the problem characteristics. Possible values are:



*	Automatic
*	Interior-Direct
*	Interior-CG
*	Active-Set
*	SQP
*	Multi-algorithm




Nonlinear programming subproblems use the algorithm specified by the option **Algorithm** . For more information about the algorithms, see the help of that option.





**Learn more about** 

*	:ref:`KNITRO_General_-_Algorithm`  
