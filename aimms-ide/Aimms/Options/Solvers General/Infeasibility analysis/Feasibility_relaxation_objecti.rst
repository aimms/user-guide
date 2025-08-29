

.. _option-AIMMS-feasibility_relaxation_objective:


Feasibility Relaxation Objective
================================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Sum of violations	



This option will set the objective for the minimum cost relaxation performed by FeasOpt (CPLEX) or FeasRelax (Gurobi). 
Possible values are:

    *	Sum of violations
    *	Sum of squared violations
    *	Number of violations


The weights are the the violation penalty values that are provided to the Mathematical Program. 

    *	For 'Sum of violations', the objective of the feasibility relaxation is to minimize the weighted sum of the constraint and bound violations.
    *	For 'Sum of squared violations', the objective is to minimize the weighted sum of squared violations. 
    *	For 'Number of violations', the weighted number of relaxed constraints and bounds is minimized. 


**Note** 


*	This option is only relevant if the option **Feasibility Relaxation** is set to 'Advanced'. 


**Learn more about** 

*	`Infeasibility analysis <https://documentation.aimms.com/language-reference/optimization-modeling-components/solving-mathematical-programs/infeasibility-analysis.html>`_ (Language Reference)
*	:ref:`option-AIMMS-feasibility_relaxation`  
*	:ref:`option-AIMMS-feasibility_relaxation_optimize_original_objective`  

