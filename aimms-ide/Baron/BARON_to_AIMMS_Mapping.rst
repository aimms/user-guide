

.. _BARON_to_AIMMS_Mapping:


BARON to AIMMS Mapping
=========================

**Description** 

The table shows in the left column the parameters from BARON that can be set in AIMMS; the right column displays for each BARON parameter the associated AIMMS option.

.. list-table::

   * - **Name in BARON**
     - **Option name in AIMMS**
   * - AbsConFeasTol
     - :ref:`option-Baron-absolute_feasibility_tolerance`
   * - AbsIntFeasTol
     - :ref:`option-Baron-absolute_integrality_tolerance`
   * - autobounds
     - :ref:`option-Baron-automatically_set_missing_bounds`
   * - boxtol
     - :ref:`option-Baron-box_elimination_tolerance`
   * - brptstra
     - :ref:`option-Baron-point_selection_strategy`
   * - brvarstra
     - :ref:`option-Baron-variable_selection_strategy`
   * - compiis
     - :ref:`option-Baron-compute_iis`
   * - cutoff
     - :ref:`option-Baron-cut_off`
   * - DeltaA
     - :ref:`option-Baron-absolute_improvement_tolerance`
   * - DeltaD
     - :ref:`option-Baron-relative_improvement_tolerance`
   * - DeltaT
     - :ref:`option-Baron-insufficient_progress_time`
   * - DeltaTerm
     - :ref:`option-Baron-insufficient_progress_termination`
   * - dolocal
     - :ref:`option-Baron-upper_bounding`
   * - epsa
     - :ref:`option-Baron-absolute_termination_tolerance`
   * - epsr
     - :ref:`option-Baron-relative_termination_tolerance`
   * - firstfeas
     - :ref:`option-Baron-find_feasible_solution_only`
   * - firstloc
     - :ref:`option-Baron-local_solution`
   * - iisint
     - :ref:`option-Baron-iis_include_integers`
   * - isoltol
     - :ref:`option-Baron-solution_distance`
   * - lbttdo
     - :ref:`option-Baron-feasibility_based_tightening`
   * - locres
     - :ref:`option-Baron-print_local_search_information`
   * - lpalg
     - :ref:`option-Baron-lp_algorithm`
   * - lpsol
     - :ref:`option-Baron-lp_solver`
   * - maxiter
     - :ref:`Options_Stop_Criteria_-_Iteration_Limi`   (General solvers option)
   * - maxtime
     - :ref:`Options_Stop_Criteria_-_Time_Limit`   (General solvers option)
   * - mdo
     - :ref:`option-Baron-marginals_testing`
   * - nlpsol
     - :ref:`option-Baron-nlp_solver`
   * - nodesel
     - :ref:`option-Baron-node_selection`
   * - nouter1
     - :ref:`option-Baron-number_of_outer_approximators`
   * - noutiter
     - :ref:`option-Baron-number_of_cutting_plane_rounds`
   * - noutpervar
     - :ref:`option-Baron-number_of_outer_approximators_multi`
   * - numloc
     - :ref:`option-Baron-number_of_preprocessing_searches`
   * - numsol
     - :ref:`option-Baron-number_of_best_solutions`
   * - obttdo
     - :ref:`option-Baron-optimality_based_tightening`
   * - outgrid
     - :ref:`option-Baron-number_of_grid_points`
   * - pdo
     - :ref:`option-Baron-number_of_probing_problems`
   * - prtimefreq
     - :ref:`option-AIMMS-progress_time_interval`   (General solvers option)
   * - RelConFeasTol
     - :ref:`option-Baron-relative_feasibility_tolerance`
   * - RelIntFeasTol
     - :ref:`option-Baron-relative_integrality_tolerance`
   * - tdo
     - :ref:`option-Baron-bounds_tightening`
   * - threads
     - :ref:`option-Baron-thread_limit_mip`
