

.. _option-AIMMS-feasibility_relaxation_optimize_original_objective:


Feasibility Relaxation Optimize Original Objective
==================================================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Off	



This option determines whether FeasOpt (ref:`SolverCPLEX`) or FeasRelax (:ref:`SolverGurobi`) should
optimize the original objective, after finding a minimum cost relaxation. Possible values are:

    *	Off
    *	On


If the option is set to 'Off', FeasOpt or FeasRelax will return a solution that minimizes the cost of the violations. 

If the option is set to 'On', FeasOpt or FeasRelax will optimize the original objective, among all solutions that
minimize the cost of the violations. 


**Note** 


*	This option is only relevant if the option **Feasibility Relaxation**  is set to 'Advanced'. 


**Learn more about** 

*	`Infeasibility analysis <https://documentation.aimms.com/language-reference/optimization-modeling-components/solving-mathematical-programs/infeasibility-analysis.html>`_ (Language Reference)
*	:ref:`option-AIMMS-feasibility_relaxation`  
*	:ref:`option-AIMMS-feasibility_relaxation_objective`  

