.. _option-KNITRO-mip_algorithm:


MIP Algorithm
=============



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Automatic	



This option specifies which algorithm to use for solving linear programming (LP) subproblem solves that may occur in the branch and bound procedure. At the default setting Knitro will automatically try to choose the best algorithm based on the problem characteristics. Possible values are:



    *	Automatic
    *	Interior-Direct
    *	Interior-CG
    *	Active-Set




In the hybrid Quesada-Grossman algorithm (see option **MIP Method**), most of the subproblems are LP subproblems and this option controls which algorithm is used for solving these LP subproblems.





The algorithm used for the nonlinear problem at the root node is specified by the option **MIP Start Algorithm**. Nonlinear programming subproblems use the algorithm specified by the option **Node Algorithm**.





See the option **Algorithm**  for more information about the algorithms.





**Learn more about** 

*	:ref:`option-KNITRO-algorithm`  
*	:ref:`option-KNITRO-mip_method`  
*	:ref:`option-KNITRO-mip_start_algorithm`  
*	:ref:`option-KNITRO-node_algorithm`  
