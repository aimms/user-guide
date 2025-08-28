.. _option-KNITRO-multistart:


Multistart
==========



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Off	



This option determines whether Knitro will solve from multiple start points to find a better local minimum. The default behavior of Knitro is to return the first locally optimal point found. Knitro offers a simple multistart feature that searches for a better optimal point by restarting Knitro from different initial points. Possible values are:



    *	Off
    *	On




The multistart procedure generates new start points by randomly selecting x components that satisfy the variable bounds. The number of start points to try is specified with the option **Number of Multistart Points**. Knitro finds a local optimum from each start point. The solution returned by Knitro is the local optimum with the best objective function value.





Knitro cannot guarantee that multistart will find the global optimum. The probability of finding a better point improves if more start points are tried, but so does the execution time. Search time can be improved if the variable bounds are made as tight as possible. Minimally, all variables need to be given finite upper and lower bounds.





The option **Number of Threads**  can be used to let the multistart algorithm run in parallel.





By default the multistart algorithm is deterministic. This is controlled by the options **Multistart Deterministic**  and **Multistart Termination Condition**.





**Note** 

*	If this option is switched on then Knitro will ignore the initial point provided by the user.




**Learn more about** 

*	:ref:`option-KNITRO-multistart_deterministic`  
*	:ref:`option-KNITRO-multistart_termination_condition`  
*	:ref:`option-KNITRO-number_of_multistart_points`  
*	:ref:`option-KNITRO-number_of_threads` 
