

.. _BARON_to_AIMMS_Mapping:


BARON to AIMMS Mapping
=========================

**Description** 

The table shows in the left column the parameters from BARON that can be set in AIMMS; the right column displays for each BARON parameter the associated AIMMS option.

.. list-table::

   * - **Name in BARON**
     - **Option name in AIMMS**
   * - AbsConFeasTol
     - :ref:`Tolerances - Absolute feasibility tolerance <option-Baron-absolute_feasibility_tolerance>`
   * - AbsIntFeasTol
     - :ref:`Tolerances - Absolute integrality tolerance <option-Baron-absolute_integrality_tolerance>`
   * - autobounds
     - :ref:`General - Automatically set missing bounds <option-Baron-automatically_set_missing_bounds>`
   * - boxtol
     - :ref:`Tolerances - Box elimination tolerance <option-Baron-box_elimination_tolerance>`
   * - brptstra
     - :ref:`Branching - Point selection strategy <option-Baron-point_selection_strategy>`
   * - brvarstra
     - :ref:`Branching - Variable selection strategy <option-Baron-variable_selection_strategy>`
   * - compiis
     - :ref:`General - Compute IIS <option-Baron-compute_iis>`
   * - cutoff
     - :ref:`General - Cut off <option-Baron-cut_off>`
   * - DeltaA
     - :ref:`Termination - Absolute improvement tolerance <option-Baron-absolute_improvement_tolerance>`
   * - DeltaD
     - :ref:`Termination - Relative improvement tolerance <option-Baron-relative_improvement_tolerance>`
   * - DeltaT
     - :ref:`Termination - Insufficient progress time <option-Baron-insufficient_progress_time>`
   * - DeltaTerm
     - :ref:`Termination - Insufficient progress termination <option-Baron-insufficient_progress_termination>`
   * - dolocal
     - :ref:`Local Search Heuristic - Upper bounding <option-Baron-upper_bounding>`
   * - epsa
     - :ref:`Termination - Absolute termination tolerance <option-Baron-absolute_termination_tolerance>`
   * - epsr
     - :ref:`Termination - Relative termination tolerance <option-Baron-relative_termination_tolerance>`
   * - firstfeas
     - :ref:`General - Find feasible solution only <option-Baron-find_feasible_solution_only>`
   * - firstloc
     - :ref:`General - Local solution <option-Baron-local_solution>`
   * - iisint
     - :ref:`General - IIS include integers <option-Baron-iis_include_integers>`
   * - isoltol
     - :ref:`General - Solution distance <option-Baron-solution_distance>`
   * - lbttdo
     - :ref:`Range Reduction - Feasibility based tightening <option-Baron-feasibility_based_tightening>`
   * - locres
     - :ref:`Logging - Print local search information <option-Baron-print_local_search_information>`
   * - lpalg
     - :ref:`General - LP algorithm <option-Baron-lp_algorithm>`
   * - lpsol
     - :ref:`General - LP solver <option-Baron-lp_solver>`
   * - maxiter
     - :ref:`Stop Criteria - Iteration Limit <option-AIMMS-iteration_limit>`   (General solvers option)
   * - maxtime
     - :ref:`Stop Criteria - Time Limit <option-AIMMS-time_limit>`   (General solvers option)
   * - mdo
     - :ref:`Range Reduction - Marginals testing <option-Baron-marginals_testing>`
   * - nlpsol
     - :ref:`General - NLP solver <option-Baron-nlp_solver>`
   * - nodesel
     - :ref:`Branching - Node selection <option-Baron-node_selection>`
   * - nouter1
     - :ref:`Relaxation - Number of outer approximators <option-Baron-number_of_outer_approximators>`
   * - noutiter
     - :ref:`Relaxation - Number of cutting plane rounds <option-Baron-number_of_cutting_plane_rounds>`
   * - noutpervar
     - :ref:`Relaxation - Number of outer approximators multi <option-Baron-number_of_outer_approximators_multi>`
   * - numloc
     - :ref:`Local Search Heuristic - Number of preprocessing searches <option-Baron-number_of_preprocessing_searches>`
   * - numsol
     - :ref:`General - Number of best solutions <option-Baron-number_of_best_solutions>`
   * - obttdo
     - :ref:`Range Reduction - Optimality based tightening <option-Baron-optimality_based_tightening>`
   * - outgrid
     - :ref:`Relaxation - Number of grid points <option-Baron-number_of_grid_points>`
   * - pdo
     - :ref:`Range Reduction - Number of probing problems <option-Baron-number_of_probing_problems>`
   * - prtimefreq
     - :ref:`Progress Options - Progress Time Interval <option-AIMMS-progress_time_interval>`   (General solvers option)
   * - RelConFeasTol
     - :ref:`Tolerances - Relative feasibility tolerance <option-Baron-relative_feasibility_tolerance>`
   * - RelIntFeasTol
     - :ref:`Tolerances - Relative integrality tolerance <option-Baron-relative_integrality_tolerance>`
   * - tdo
     - :ref:`Range Reduction - Bounds tightening <option-Baron-bounds_tightening>`
   * - threads
     - :ref:`Parallel - Thread limit MIP <option-Baron-thread_limit_mip>`
