.. _option-GUROBI-pdhg_relative_feasibility_tolerance:


PDHG Relative Feasibility Tolerance
===================================



:Type:	Floating point number	
:Range:	[0.0,1e100]	
:Default:	1e-6	



The PDHG algorithm will terminate if the absolute residuals of all primal and dual equations are below the value of this option.

Other termination criteria are specified by the options **PDHG Absolute Feasibility Tolerance** and **PDHG Convergence Tolerance**.

If you set this option to the special value zero (0), then only the absolute feasibility tolerances are considered. Specifically,
primal and dual solutions are considered feasible only if the residuals of all primal and dual equations are below the value
of the option **PDHG Absolute Feasibility Tolerance**.


**Note** 

*	This option was added in Gurobi 13.0.


**Learn more about** 

*	:ref:`option-GUROBI-pdhg_absolute_feasibility_tolerance`  
*	:ref:`option-GUROBI-pdhg_convergence_tolerance`  

