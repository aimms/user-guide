.. _option-CPLEX-sensitivity_method:


Sensitivity Method
==================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Dual simplex	



This option specifies which method is used by CPLEX for solving LP problems while calculating sensitivity ranges. Possible values are:

    *	Primal simplex
    *	Dual simplex
    *	Network + Primal (*network followed by primal simplex*)
    *	Network + Dual (*network followed by dual simplex*)
    *	Barrier
    *	Sifting
    *	Concurrent


See the option **LP Method** for a description of the algorithms.


Multiple LP problems are solved to calculate shadow price ranges for constraints and value ranges for variables.
See :ref:`Miscellaneous_Calculation_of_Shadow_Price_Ra` for more information.


**Note** 

*	The barrier algorithm can use multiple threads as controlled by the option **Global Thread Limit**.


**Learn more about** 

*	:ref:`option-AIMMS-calculate_sensitivity_ranges` 
*	:ref:`option-CPLEX-global_thread_limit`  
*	:ref:`option-CPLEX-lp_method` 

