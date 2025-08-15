

.. _BARON_to_AIMMS_Mapping:


BARON to AIMMS Mapping
=========================

**Description** 

The table shows in the left column the parameters from BARON that can be set in AIMMS; the right column displays for each BARON parameter the associated AIMMS option.

.. list-table::

   * - **Name in BARON**
     - **Option name in AIMMS**
   * - AbsConFeasTol
     - :ref:`Baron_Tolerances_-_Absolute_feasibility_tolerance`
   * - AbsIntFeasTol
     - :ref:`Baron_Tolerances_-_Absolute_Integrality_toler`
   * - autobounds
     - :ref:`Baron_General_-_Automatically_set_mi`
   * - boxtol
     - :ref:`Baron_Tolerances_-_Box_elimination_t`
   * - brptstra
     - :ref:`Baron_Branching_-_Point_selection_st`
   * - brvarstra
     - :ref:`Baron_Branching_-_Variable_selection`
   * - compiis
     - :ref:`Baron_General_-_Compute_IIS`
   * - cutoff
     - :ref:`Baron_General_-_Cutoff`
   * - DeltaA
     - :ref:`Baron_Termination_-_Absolute_improvement_tolerance`
   * - DeltaD
     - :ref:`Baron_Termination_-_Relative_improvement_tolerance`
   * - DeltaT
     - :ref:`Baron_Termination_-_Insufficient_progress_time`
   * - DeltaTerm
     - :ref:`Baron_Termination_-_Insufficient_progress_terminat`
   * - dolocal
     - :ref:`Baron_Local_Search_Heuristic_-_Upper`
   * - epsa
     - :ref:`Baron_Termination_-_Absolute_terminat`
   * - epsr
     - :ref:`Baron_Termination_-_Relative_terminat`
   * - firstfeas
     - :ref:`Baron_General_-_Find_feasible_soluti`
   * - firstloc
     - :ref:`Baron_General_-_Local_solution`
   * - iisint
     - :ref:`Baron_General_-_IIS_include_integers`
   * - isoltol
     - :ref:`Baron_General_-_Solutiondistance`
   * - lbttdo
     - :ref:`Baron_Range_Reduction_-_Feasibility_`
   * - locres
     - :ref:`Baron_Logging_-_Print_local_search_i`
   * - lpalg
     - :ref:`Baron_General_-_LP_algorithm`
   * - lpsol
     - :ref:`Baron_General_-_LP_solver`
   * - maxiter
     - :ref:`Options_Stop_Criteria_-_Iteration_Limi`   (General solvers option)
   * - maxtime
     - :ref:`Options_Stop_Criteria_-_Time_Limit`   (General solvers option)
   * - mdo
     - :ref:`Baron_Range_Reduction_-_Marginals_te`
   * - nlpsol
     - :ref:`Baron_General_-_NLP_solver`
   * - nodesel
     - :ref:`Baron_Branching_-_Node_select`
   * - nouter1
     - :ref:`Baron_Relaxation_-_Number_of_outer_a`
   * - noutiter
     - :ref:`Baron_Relaxation_-_Number_of_cutting`
   * - noutpervar
     - :ref:`Baron_Relaxation_-_Number_of_outer_approximators_m`
   * - numloc
     - :ref:`Baron_Local_Search_Heuristic_-_Numbe`
   * - numsol
     - :ref:`Baron_General_-_Numberofbestsolutio`
   * - obttdo
     - :ref:`Baron_Range_Reduction_-_Optimality_b`
   * - outgrid
     - :ref:`Baron_Relaxation_-_Number_of_grid_points`
   * - pdo
     - :ref:`Baron_Range_Reduction_-_Number_of_pr`
   * - prtimefreq
     - :ref:`Options_Progress_Options_-_Progress_Time_Interval`   (General solvers option)
   * - RelConFeasTol
     - :ref:`Baron_Tolerances_-_Relative_feasibility_tolerance`
   * - RelIntFeasTol
     - :ref:`Baron_Tolerances_-_Relative_Integrality_toler`
   * - tdo
     - :ref:`Baron_Range_Reduction_-_Bounds_tight`
   * - threads
     - :ref:`Baron_Parallel_-_Thread_limit_MIP`
