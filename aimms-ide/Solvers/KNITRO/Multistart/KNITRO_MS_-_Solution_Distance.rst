.. _option-KNITRO-solution_distance:


Solution Distance
=================



:Type:	Floating point number	
:Range:	[0,1e20]	
:Default:	Na



This option specifies the tolerance for deciding if two feasible points are distinct. Points are distinct if they differ in objective value or some component (i.e., level value or Lagrange multiplier) by the value of this option. A large value can cause the saved feasible points to cluster around more widely separated points. The default value of this option is the machine precision, and depends on the machine.



This is a relative tolerance. Two components x and y are considered equal if
	abs(x-y) ≤ abs(x)*tol,



where tol is the value of this option.



This option has only effect if option **Number of Best Solutions**  is activated and if the option **Multistart**  is switched on.



**Learn more about** 

*	:ref:`option-KNITRO-multistart`  
*	:ref:`option-KNITRO-number_of_best_solutions`  
