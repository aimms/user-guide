.. _option-KNITRO-linear_solver_out_of_core:


Linear Solver Out of Core
=========================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Off	



This option indicates whether to solve linear systems out-of-core when using Intel MKL PARDISO. This option is only active if the option **Linear Solver**  is set to 'MKL PARDISO'. Possible values are:



*	Off
*	Automatic
*	On




With setting 'Automatic' Knitro bases the decision to solve out-of-core depending on how much space is needed.





**Learn more about** 

*	:ref:`option-KNITRO-linear_solver` 
