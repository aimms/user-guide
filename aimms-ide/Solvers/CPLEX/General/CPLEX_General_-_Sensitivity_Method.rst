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
See :doc:`../../../Aimms/Miscellaneous/Short Descriptions/Calculation_of_Shadow_Price_Ra` for more information.


**Note** 

*	The barrier algorithm can use multiple threads as controlled by the option **Global Thread Limit**.


**Learn more about** 

*	:doc:`../../../Aimms/Options/Solvers General/Sensitivity/Sensitivity_-_Calculate_Sensit` 
*	:doc:`../Parallel/CPLEX_Par_-_GlobalThreadLimit`  
*	:doc:`CPLEX_General_-_LP_Method` 

