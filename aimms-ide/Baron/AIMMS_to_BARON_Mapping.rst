

.. _AIMMS_to_BARON_Mapping:


AIMMS to BARON Mapping
=========================

**Description** 

The table shows in the left column the AIMMS BARON options; the right column display for the AIMMS options the BARON parameter that is associated with it.

.. list-table::

   * - **Option name in AIMMS**
     - **Name in BARON**
   * - :ref:`option-Baron-point_selection_strategy`
     - brptstra
   * - :ref:`option-Baron-node_selection`
     - nodesel
   * - :ref:`option-Baron-variable_selection_strategy`
     - brvarstra
   * - :ref:`option-Baron-automatically_set_missing_bounds`
     - autobounds
   * - :ref:`option-Baron-compute_iis`
     - compiis
   * - :ref:`option-Baron-cut_off`
     - cutoff
   * - :ref:`option-Baron-find_feasible_solution_only`
     - firstfeas
   * - :ref:`option-Baron-iis_include_integers`
     - iisint
   * - :ref:`option-Baron-local_solution`
     - firstloc
   * - :ref:`option-Baron-lp_algorithm`
     - lpalg
   * - :ref:`option-Baron-lp_solver`
     - lpsol
   * - :ref:`option-Baron-nlp_solver`
     - nlpsol
   * - :ref:`option-Baron-number_of_best_solutions`
     - numsol
   * - :ref:`option-Baron-solution_distance`
     - isoltol
   * - :ref:`option-Baron-number_of_preprocessing_searches`
     - numloc
   * - :ref:`option-Baron-upper_bounding`
     - dolocal
   * - :ref:`option-Baron-print_local_search_information`
     - locres
   * - :ref:`option-Baron-thread_limit_mip`
     - threads
   * - :ref:`option-Baron-bounds_tightening`
     - tdo
   * - :ref:`option-Baron-feasibility_based_tightening`
     - lbttdo
   * - :ref:`option-Baron-marginals_testing`
     - mdo
   * - :ref:`option-Baron-number_of_probing_problems`
     - pdo
   * - :ref:`option-Baron-optimality_based_tightening`
     - obttdo
   * - :ref:`option-Baron-number_of_cutting_plane_rounds`
     - noutiter
   * - :ref:`option-Baron-number_of_grid_points`
     - outgrid
   * - :ref:`option-Baron-number_of_outer_approximators`
     - nouter1
   * - :ref:`option-Baron-number_of_outer_approximators_multi`
     - noutpervar
   * - :ref:`option-Baron-absolute_improvement_tolerance`
     - DeltaA
   * - :ref:`option-Baron-absolute_termination_tolerance`
     - epsa
   * - :ref:`option-Baron-insufficient_progress_termination`
     - DeltaTerm
   * - :ref:`option-Baron-insufficient_progress_time`
     - DeltaT
   * - :ref:`option-Baron-relative_improvement_tolerance`
     - DeltaD
   * - :ref:`option-Baron-relative_termination_tolerance`
     - epsr
   * - :ref:`option-Baron-absolute_feasibility_tolerance`
     - AbsConFeasTol
   * - :ref:`option-Baron-absolute_integrality_tolerance`
     - AbsIntFeasTol
   * - :ref:`option-Baron-box_elimination_tolerance`
     - boxtol
   * - :ref:`option-Baron-relative_feasibility_tolerance`
     - RelConFeasTol
   * - :ref:`option-Baron-relative_integrality_tolerance`
     - RelIntFeasTol
