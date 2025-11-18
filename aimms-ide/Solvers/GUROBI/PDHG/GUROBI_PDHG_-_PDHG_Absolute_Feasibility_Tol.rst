.. _option-GUROBI-pdhg_absolute_feasibility_tolerance:


PDHG Absolute Feasibility Tolerance
===================================



:Type:	Floating point number	
:Range:	[1e-9,1e-2]	
:Default:	1e-6	



The PDHG algorithm will terminate if the relative residuals of all primal and dual equations are below the value of this option.

Other termination criteria are specified by the options **PDHG Convergence Tolerance** and **PDHG Relative Feasibility Tolerance**.

Note though that relative tolerances typically lead to earlier termination than absolute tolerances. If you wish to terminate PDHG
based solely on absolute tolerances, you should set the option **PDHG Relative Feasibility Tolerance** to zero (0).


**Note** 

*	This option was added in Gurobi 13.0.


**Learn more about** 

*	:ref:`option-GUROBI-pdhg_convergence_tolerance`  
*	:ref:`option-GUROBI-pdhg_relative_feasibility_tolerance`  

