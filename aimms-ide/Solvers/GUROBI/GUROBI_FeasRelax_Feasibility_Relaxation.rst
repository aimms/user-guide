.. _GUROBI_FeasRelax_Feasibility_Relaxation:


FeasRelax (Feasibility Relaxation)
==================================

Gurobi allows the calculation of a minimum-cost relaxation for a given mathematical program. A minimum-cost relaxation of an infeasible model is a solution that minimizes the weighted amount by which it violates the variable bounds and constraints. The weights are the penalty values that are specified for the current model. 



Feasibility relaxation can be enabled by adding penalty values to the mathematical program and setting the option :ref:`option-AIMMS-feasibility_relaxation` to 'Advanced' (keeping the option at 'Standard' will apply the regular AIMMS method of violation penalties).



Feasibility relaxation allows several options for the objective in the minimum-cost relaxation. The options are:




*   Minimize the weighted sum of the penalties for the relaxations. 
*   Minimize the weighted sum of squared penalties of the relaxations. 
*   Minimze the weighted number of relaxed bounds and constraints. 



Here, the weights are the penalty values that are specified for the mathematical program. 



The objective for the minimum-cost relaxation can be set using the option :ref:`option-AIMMS-feasibility_relaxation_objective`. 



After computing a minimum-cost relaxation (also referred to as 'Phase I'), Gurobi can optionally optimize the original objective among all solutions with a minimum-cost relaxation ('Phase II'). This can be enabled by setting the option :ref:`option-AIMMS-feasibility_relaxation_optimize_original_objective`.



If this option is disabled, AIMMS will stop after Phase I and return a minimum-cost relaxation. If the option is enabled, AIMMS will continue to Phase II and return a solution that optimizes the original objective, among all solutions with a minimum cost violation. 



**Note** 

*	Feasibility relaxation is not enabled for lazy pool, cut pool, quadratic and indicator constraints. 
*	In case the objective 'Minimize the weighted number of relaxed bounds and constraints' is selected, if the problem was a Linear Program, it will be transformed into a Mixed Integer Program. 
*	In case the objective 'Minimize the weighted sum of squared penalties of the relaxations' is selected, if the problem was a Linear Program, it will be transformed into a Quadratic Program. 




**Learn more about** 


· 	`Violation penalties <https://documentation.aimms.com/language-reference/optimization-modeling-components/solving-mathematical-programs/infeasibility-analysis.html>`_ (Language Reference)

*	:ref:`option-AIMMS-feasibility_relaxation` 
*	:ref:`option-AIMMS-feasibility_relaxation_objective` 
*	:ref:`option-AIMMS-feasibility_relaxation_optimize_original_objective` 
*	:ref:`option-GUROBI-feasrelax_big_m` 



