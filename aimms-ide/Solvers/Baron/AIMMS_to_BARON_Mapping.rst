

.. _AIMMS_to_BARON_Mapping:


AIMMS to BARON Mapping
=========================

**Description** 

The table shows in the left column the AIMMS BARON options; the right column display for the AIMMS options the BARON parameter that is associated with it.

.. list-table::

   * - **Option name in AIMMS**
     - **Name in BARON**
   * - :ref:`Branching - Point selection strategy <option-Baron-point_selection_strategy>`
     - brptstra
   * - :ref:`Branching - Node selection <option-Baron-node_selection>`
     - nodesel
   * - :ref:`Branching - Variable selection strategy <option-Baron-variable_selection_strategy>`
     - brvarstra
   * - :ref:`General - Automatically set missing bounds <option-Baron-automatically_set_missing_bounds>`
     - autobounds
   * - :ref:`General - Compute IIS <option-Baron-compute_iis>`
     - compiis
   * - :ref:`General - Cut off <option-Baron-cut_off>`
     - cutoff
   * - :ref:`General - Find feasible solution only <option-Baron-find_feasible_solution_only>`
     - firstfeas
   * - :ref:`General - IIS include integers <option-Baron-iis_include_integers>`
     - iisint
   * - :ref:`General - Local solution <option-Baron-local_solution>`
     - firstloc
   * - :ref:`General - LP algorithm <option-Baron-lp_algorithm>`
     - lpalg
   * - :ref:`General - LP solver <option-Baron-lp_solver>`
     - lpsol
   * - :ref:`General - NLP solver <option-Baron-nlp_solver>`
     - nlpsol
   * - :ref:`General - Number of best solutions <option-Baron-number_of_best_solutions>`
     - numsol
   * - :ref:`General - Solution distance <option-Baron-solution_distance>`
     - isoltol
   * - :ref:`Local Search Heuristic - Number of preprocessing searches <option-Baron-number_of_preprocessing_searches>`
     - numloc
   * - :ref:`Local Search Heuristic - Upper bounding <option-Baron-upper_bounding>`
     - dolocal
   * - :ref:`Logging - Print local search information <option-Baron-print_local_search_information>`
     - locres
   * - :ref:`Parallel - Thread limit MIP <option-Baron-thread_limit_mip>`
     - threads
   * - :ref:`Range Reduction - Bounds tightening <option-Baron-bounds_tightening>`
     - tdo
   * - :ref:`Range Reduction - Feasibility based tightening <option-Baron-feasibility_based_tightening>`
     - lbttdo
   * - :ref:`Range Reduction - Marginals testing <option-Baron-marginals_testing>`
     - mdo
   * - :ref:`Range Reduction - Number of probing problems <option-Baron-number_of_probing_problems>`
     - pdo
   * - :ref:`Range Reduction - Optimality based tightening <option-Baron-optimality_based_tightening>`
     - obttdo
   * - :ref:`Relaxation - Number of cutting plane rounds <option-Baron-number_of_cutting_plane_rounds>`
     - noutiter
   * - :ref:`Relaxation - Number of grid points <option-Baron-number_of_grid_points>`
     - outgrid
   * - :ref:`Relaxation - Number of outer approximators <option-Baron-number_of_outer_approximators>`
     - nouter1
   * - :ref:`Relaxation - Number of outer approximators multi <option-Baron-number_of_outer_approximators_multi>`
     - noutpervar
   * - :ref:`Termination - Absolute improvement tolerance <option-Baron-absolute_improvement_tolerance>`
     - DeltaA
   * - :ref:`Termination - Absolute termination tolerance <option-Baron-absolute_termination_tolerance>`
     - epsa
   * - :ref:`Termination - Insufficient progress termination <option-Baron-insufficient_progress_termination>`
     - DeltaTerm
   * - :ref:`Termination - Insufficient progress time <option-Baron-insufficient_progress_time>`
     - DeltaT
   * - :ref:`Termination - Relative improvement tolerance <option-Baron-relative_improvement_tolerance>`
     - DeltaD
   * - :ref:`Termination - Relative termination tolerance <option-Baron-relative_termination_tolerance>`
     - epsr
   * - :ref:`Tolerances - Absolute feasibility tolerance <option-Baron-absolute_feasibility_tolerance>`
     - AbsConFeasTol
   * - :ref:`Tolerances - Absolute integrality tolerance <option-Baron-absolute_integrality_tolerance>`
     - AbsIntFeasTol
   * - :ref:`Tolerances - Box elimination tolerance <option-Baron-box_elimination_tolerance>`
     - boxtol
   * - :ref:`Tolerances - Relative feasibility tolerance <option-Baron-relative_feasibility_tolerance>`
     - RelConFeasTol
   * - :ref:`Tolerances - Relative integrality tolerance <option-Baron-relative_integrality_tolerance>`
     - RelIntFeasTol
