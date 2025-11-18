.. _option-GUROBI-sensitivity_method:


Sensitivity Method
==================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Automatic	



This option specifies which method is used by Gurobi for solving LP problems while calculating sensitivity ranges. Possible values are:

    *	Automatic
    *	Primal simplex
    *	Dual simplex
    *	Barrier
    *	Opportunistic concurrent
    *	Deterministic concurrent
    *	PDHG


See the option **Method** for a description of the algorithms.

Multiple LP problems are solved to calculate shadow price ranges for constraints and value ranges for variables. See
:ref:`Miscellaneous_Calculation_of_Shadow_Price_Ra` for more information.


**Note** 

*	The option **Concurrent Method** controls the methods used by the concurrent solver.
*	The Primal-Dual Hybrid Gradient (PDHG) algorithm was added in Gurobi 13.0.


**Learn more about** 

*	:ref:`option-AIMMS-calculate_sensitivity_ranges` 
*	:ref:`option-GUROBI-concurrent_method` 
*	:ref:`option-GUROBI-method` 

