.. _option-KNITRO-crossover_iterations_limit:


Crossover Iterations Limit
==========================



:Type:	Integer	
:Range:	{0..1000000}	
:Default:	0	



This option determines the maximum number of crossover iterations before termination.



Interior point (or barrier) methods are a powerful tool for solving large-scale optimization problems. However, one drawback of these methods, in contrast to active-set methods, is that they do not always provide a clear picture of which constraints are active at the solution and in general they return a less exact solution and less exact sensitivity information. For this reason, Knitro offers a crossover feature in which the interior point method switches to the active-set method at the interior-point solution estimate, in order to try to "clean up" the solution and provide more exact sensitivity and active-set information.



The crossover procedure is controlled by this option. Let n denote the value of this option. If n is greater than 0, then Knitro will attempt to perform n active-set crossover iterations after the interior-point method has finished, to see if it can provide a more exact solution. This can be viewed as a form of post-processing. If n equals 0, then no crossover iterations are attempted. By default, no crossover iterations are performed.



The crossover procedure will not always succeed in obtaining a more exact solution compared with the interior-point solution. If crossover is unable to improve the solution within n crossover iterations, then it will restore the interior-point solution estimate and terminate. If the option **Status File Display**  is switched on and not set equal to 'Summary', Knitro will print a message in the status file indicating that it was unable to improve the solution. For example, if n=3, and the crossover procedure did not succeed within 3 iterations, the message will read:



	Crossover mode unable to improve solution within 3 iterations.



In this case, you may want to increase the value of this option and try again. If it appears that the crossover procedure will not succeed, no matter how many iterations are tried, then a message of the form



	Crossover mode unable to improve solution.



will be printed in the status file.



The extra cost of performing crossover is problem dependent. In most small or medium scale problems, the crossover cost should be a small fraction of the total solve cost. In these cases it may be worth using the crossover procedure to obtain a more exact solution. On some large scale or difficult degenerate problems, however, the cost of performing crossover may be significant. It is recommended to experiment with this option to see whether the improvement in the exactness of the solution is worth the additional cost.



**Learn more about** 

*	:ref:`option-KNITRO-algorithm`  
*	:ref:`option-KNITRO-status_file_display`  



