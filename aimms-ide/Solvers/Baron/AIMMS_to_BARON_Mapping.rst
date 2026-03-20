

.. _AIMMS_to_BARON_Mapping:


AIMMS to BARON Mapping
=========================

**Description** 

The table shows in the left column the AIMMS BARON options; the right column display for the AIMMS options the BARON parameter that is associated with it.

.. list-table::

   * - **Option name in AIMMS**
     - **Name in BARON**
   * - :doc:`Branching - Point selection strategy <Branching/BARON_Branching_-_Point_selection_st>`
     - brptstra
   * - :doc:`Branching - Node selection <Branching/BARON_Branching_-_Node_select>`
     - nodesel
   * - :doc:`Branching - Variable selection strategy <Branching/BARON_Branching_-_Variable_selection>`
     - brvarstra
   * - :doc:`General - Automatically set missing bounds <General/BARON_General_-_Automatically_set_mi>`
     - autobounds
   * - :doc:`General - Compute IIS <General/BARON_General_-_Compute_IIS>`
     - compiis
   * - :doc:`General - Cut off <General/BARON_General_-_Cutoff>`
     - cutoff
   * - :doc:`General - Find feasible solution only <General/BARON_General_-_Find_feasible_soluti>`
     - firstfeas
   * - :doc:`General - IIS include integers <General/BARON_General_-_IIS_include_integers>`
     - iisint
   * - :doc:`General - Local solution <General/BARON_General_-_Local_solution>`
     - firstloc
   * - :doc:`General - LP algorithm <General/BARON_General_-_LP_algorithm>`
     - lpalg
   * - :doc:`General - LP solver <General/BARON_General_-_LP_solver>`
     - lpsol
   * - :doc:`General - NLP solver <General/BARON_General_-_NLP_solver>`
     - nlpsol
   * - :doc:`General - Number of best solutions <General/BARON_General_-_Numberofbestsolutio>`
     - numsol
   * - :doc:`General - Solution distance <General/BARON_General_-_Solutiondistance>`
     - isoltol
   * - :doc:`Local Search Heuristic - Number of preprocessing searches <Local Search Heuristic/BARON_Local_Search_Heuristic_-_Numbe>`
     - numloc
   * - :doc:`Local Search Heuristic - Upper bounding <Local Search Heuristic/BARON_Local_Search_Heuristic_-_Upper>`
     - dolocal
   * - :doc:`Logging - Print local search information <Logging/BARON_Logging_-_Print_local_search_i>`
     - locres
   * - :doc:`Parallel - Thread limit MIP <Parallel/BARON_Parallel_-_Thread_limit_MIP>`
     - threads
   * - :doc:`Range Reduction - Bounds tightening <Range Reduction/BARON_Range_Reduction_-_Bounds_tight>`
     - tdo
   * - :doc:`Range Reduction - Feasibility based tightening <Range Reduction/BARON_Range_Reduction_-_Feasibility_>`
     - lbttdo
   * - :doc:`Range Reduction - Marginals testing <Range Reduction/BARON_Range_Reduction_-_Marginals_te>`
     - mdo
   * - :doc:`Range Reduction - Number of probing problems <Range Reduction/BARON_Range_Reduction_-_Number_of_pr>`
     - pdo
   * - :doc:`Range Reduction - Optimality based tightening <Range Reduction/BARON_Range_Reduction_-_Optimality_b>`
     - obttdo
   * - :doc:`Relaxation - Number of cutting plane rounds <Relaxation/BARON_Relaxation_-_Number_of_cutting>`
     - noutiter
   * - :doc:`Relaxation - Number of grid points <Relaxation/BARON_Relaxation_-_Number_of_grid_points>`
     - outgrid
   * - :doc:`Relaxation - Number of outer approximators <Relaxation/BARON_Relaxation_-_Number_of_outer_a>`
     - nouter1
   * - :doc:`Relaxation - Number of outer approximators multi <Relaxation/BARON_Relaxation_-_Number_of_outer_approximators_m>`
     - noutpervar
   * - :doc:`Termination - Absolute improvement tolerance <Termination/BARON_Termination_-_Absolute_improvement_tolerance>`
     - DeltaA
   * - :doc:`Termination - Absolute termination tolerance <Termination/BARON_Termination_-_Absolute_terminat>`
     - epsa
   * - :doc:`Termination - Insufficient progress termination <Termination/BARON_Termination_-_Insufficient_progress_terminat>`
     - DeltaTerm
   * - :doc:`Termination - Insufficient progress time <Termination/BARON_Termination_-_Insufficient_progress_time>`
     - DeltaT
   * - :doc:`Termination - Relative improvement tolerance <Termination/BARON_Termination_-_Relative_improvement_tolerance>`
     - DeltaD
   * - :doc:`Termination - Relative termination tolerance <Termination/BARON_Termination_-_Relative_terminat>`
     - epsr
   * - :doc:`Tolerances - Absolute feasibility tolerance <Tolerances/BARON_Tolerances_-_Absolute_feasibility_tolerance>`
     - AbsConFeasTol
   * - :doc:`Tolerances - Absolute integrality tolerance <Tolerances/BARON_Tolerances_-_Absolute_Integrality_toler>`
     - AbsIntFeasTol
   * - :doc:`Tolerances - Box elimination tolerance <Tolerances/BARON_Tolerances_-_Box_elimination_t>`
     - boxtol
   * - :doc:`Tolerances - Relative feasibility tolerance <Tolerances/BARON_Tolerances_-_Relative_feasibility_tolerance>`
     - RelConFeasTol
   * - :doc:`Tolerances - Relative integrality tolerance <Tolerances/BARON_Tolerances_-_Relative_Integrality_toler>`
     - RelIntFeasTol
