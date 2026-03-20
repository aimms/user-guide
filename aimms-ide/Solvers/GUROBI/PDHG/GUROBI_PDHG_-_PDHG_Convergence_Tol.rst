.. _option-GUROBI-pdhg_convergence_tolerance:


PDHG Convergence Tolerance
==========================



:Type:	Floating point number	
:Range:	[0.0,1.0]	
:Default:	1e-6	



The PDHG algorithm will terminate if the relative difference between the primal and dual objective values is less the value of this option.

Other termination criteria are specified by the options **PDHG Absolute Feasibility Tolerance** and **PDHG Relative Feasibility Tolerance**.


**Note** 

*	This option was added in Gurobi 13.0.


**Learn more about** 

*	:doc:`GUROBI_PDHG_-_PDHG_Absolute_Feasibility_Tol`  
*	:doc:`GUROBI_PDHG_-_PDHG_Relative_Feasibility_Tol`    

