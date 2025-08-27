

.. _option-AIMMS-restore_original_solution_after_analysis:


Restore Original Solution After Analysis
========================================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	No	



In the Math Program Inspector, during determination of the substructure causing unboundedness or infeasibility and during determination of an IIS, the original problem is perturbated. After the substructure or IIS has been found, the original problem is restored. With this option you can determine whether also the original solution should be restored after such an analysis step. Possible values are:



    *	No
    *	Yes




The Math Program Inspector copies the original solution before it conducts an analysis to determine the cause of infeasibility or unboundedness. If this option is set to 'Yes' then this solution will be copied back after finishing the analysis.





The substructure causing infeasibility is calculated by solving a perturbation of the original problem in which slack variables are added for all constraints and for each finite variable bound. The substructure causing unboundedness is calculated by solving a perturbation of the original problem in which finite bounds are added for all variables (except the objective variable). If this option is set at its default value then the solution of the perturbated problem will be shown in the Math Program Inspector. However, the model status will be set to 'infeasible' or 'Unbounded' (or 'InfeasibleOrUnbounded') after the analysis even though the perturbated problem is normally feasible.





The IIS is calculated by solving a sequence of problems. Also in this case the model status will be set to 'infeasible' (or 'InfeasibleOrUnbounded') after the analysis.





**Learn more about** 

*	:ref:`aimmshelp26-Math_Program_Inspector` 






