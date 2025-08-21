

.. _AIMMS_to_KNITRO_Mapping:


AIMMS to Knitro Mapping
============================

**Description** 

The table shows in the left column the AIMMS Knitro options; the right column displays for the AIMMS option the Knitro option that is associated with it.

.. list-table::

   * - **Option name in AIMMS**
     - **Name in Knitro**
   * - :ref:`option-KNITRO-estimate_noise_in_the_model`
     - findiff_estnoise
   * - :ref:`option-KNITRO-gradient_computation_method`
     - gradopt
   * - :ref:`option-KNITRO-initial_penalty_value`
     - initpenalty
   * - :ref:`option-KNITRO-initial_pivot_treshold`
     - linsolver_pivottol
   * - :ref:`option-KNITRO-initial_trust_scaling_factor`
     - delta
   * - :ref:`option-KNITRO-linesearch_strategy`
     - linesearch
   * - :ref:`option-KNITRO-linesearch_trials_limit`
     - linesearch_maxtrials
   * - :ref:`option-KNITRO-lp_algorithm`
     - act_lpalg
   * - :ref:`option-KNITRO-objective_reduction`
     - act_lppenalty
   * - :ref:`option-KNITRO-lp_presolve`
     - act_lppresolve
   * - :ref:`option-KNITRO-qp_and_qcqp_initialization_strategy`
     - ncvx_qcqp_init
   * - :ref:`option-KNITRO-solution_progress_iterations`
     - xtol_iters
   * - :ref:`option-KNITRO-solution_progress_tolerance`
     - xtol
   * - :ref:`option-KNITRO-data_check`
     - datacheck
   * - :ref:`option-KNITRO-debugging_mip_output`
     - mip_debug
   * - :ref:`option-KNITRO-debugging_output`
     - debug
   * - :ref:`option-KNITRO-act_qppenalty`
     - act_qppenalty
   * - :ref:`option-KNITRO-algorithm`
     - algorithm
   * - :ref:`option-KNITRO-blas_option`
     - blasoption
   * - :ref:`option-KNITRO-honor_bounds`
     - honorbnds
   * - :ref:`option-KNITRO-linear_solver`
     - linsolver
   * - :ref:`option-KNITRO-linear_solver_node_amalgamation`
     - linsolver_nodeamalg
   * - :ref:`option-KNITRO-linear_solver_ordering`
     - linsolver_ordering
   * - :ref:`option-KNITRO-linear_solver_out_of_core`
     - linsolver_ooc
   * - :ref:`option-KNITRO-linear_solver_scaling`
     - linsolver_scaling
   * - :ref:`option-KNITRO-linear_system_max_iterative_refinements`
     - linsolver_maxitref
   * - :ref:`option-KNITRO-lp_solver`
     - act_lpsolver
   * - :ref:`option-KNITRO-mark_as_convex`
     - convex
   * - :ref:`option-KNITRO-qp_algorithm`
     - act_qpalg
   * - :ref:`option-KNITRO-restarts`
     - restarts
   * - :ref:`option-KNITRO-restarts_iteration_limit`
     - restarts_maxit
   * - :ref:`option-KNITRO-scale_variables`
     - scale_vars
   * - :ref:`option-KNITRO-scaling`
     - scale
   * - :ref:`option-KNITRO-unboundedness_range`
     - objrange
   * - :ref:`option-KNITRO-warm_start_strategy`
     - strat_warm_start
   * - :ref:`option-KNITRO-hessian_computation_method`
     - hessopt
   * - :ref:`option-KNITRO-limited_memory_size`
     - lmsize
   * - :ref:`option-KNITRO-second_order_correction`
     - soc
   * - :ref:`option-KNITRO-barrier_corrector_steps_limit`
     - bar_maxcorrectors
   * - :ref:`option-KNITRO-barrier_enable_conic`
     - bar_conic_enable
   * - :ref:`option-KNITRO-barrier_globalize`
     - bar_globalize
   * - :ref:`option-KNITRO-barrier_maximum_mu`
     - bar_maxmu
   * - :ref:`option-KNITRO-barrier_mpec_heuristic`
     - bar_mpec_heuristic
   * - :ref:`option-KNITRO-barrier_parameter_strategy`
     - bar_murule
   * - :ref:`option-KNITRO-barrier_penalty_constraint_strategy`
     - bar_penaltycons
   * - :ref:`option-KNITRO-barrier_penalty_parameter_strategy`
     - bar_penaltyrule
   * - :ref:`option-KNITRO-barrier_refinement`
     - bar_refinement
   * - :ref:`option-KNITRO-barrier_relax_constraints`
     - bar_relaxcons
   * - :ref:`option-KNITRO-barrier_slack_bound_push`
     - bar_slackboundpush
   * - :ref:`option-KNITRO-barrier_switch_objective`
     - bar_switchobj
   * - :ref:`option-KNITRO-barrier_switch_rule`
     - bar_switchrule
   * - :ref:`option-KNITRO-barrier_watchdog`
     - bar_watchdog
   * - :ref:`option-KNITRO-conjugate_gradient_iteration_limit`
     - cg_maxit
   * - :ref:`option-KNITRO-conjugate_gradient_memory_limit`
     - cg_pmem
   * - :ref:`option-KNITRO-conjugate_gradient_preconditioner`
     - cg_precond
   * - :ref:`option-KNITRO-conjugate_gradient_stopping_tolerance`
     - cg_stoptol
   * - :ref:`option-KNITRO-crossover_iterations_limit`
     - bar_maxcrossit
   * - :ref:`option-KNITRO-direct_step_interval`
     - bar_directinterval
   * - :ref:`option-KNITRO-feasible_mode`
     - bar_feasible
   * - :ref:`option-KNITRO-feasible_mode_activation_tolerance`
     - bar_feasmodetol
   * - :ref:`option-KNITRO-initial_barrier_parameter_value`
     - bar_initmu
   * - :ref:`option-KNITRO-initial_barrier_penalty_value_mpec`
     - bar_initpi_mpec
   * - :ref:`option-KNITRO-initial_point_strategy`
     - bar_initpt
   * - :ref:`option-KNITRO-linear_system_form_used`
     - bar_linsys
   * - :ref:`option-KNITRO-linear_system_memory_usage`
     - bar_linsys_storage
   * - :ref:`option-KNITRO-refactorization_limit`
     - bar_maxrefactor
   * - :ref:`option-KNITRO-integrality`
     - mip_integer_tol
   * - :ref:`option-KNITRO-maximal_number_of_nodes`
     - mip_maxnodes
   * - :ref:`option-KNITRO-maximal_number_of_subproblem_solves`
     - mip_maxsolves
   * - :ref:`option-KNITRO-mip_algorithm`
     - mip_lpalg
   * - :ref:`option-KNITRO-mip_branching_rule`
     - mip_branchrule
   * - :ref:`option-KNITRO-mip_gub_branch`
     - mip_gub_branch
   * - :ref:`option-KNITRO-mip_heuristic`
     - mip_heuristic
   * - :ref:`option-KNITRO-mip_heuristic_diving`
     - mip_heuristic_diving
   * - :ref:`option-KNITRO-mip_heuristic_feasibility_pump`
     - mip_heuristic_feaspump
   * - :ref:`option-KNITRO-mip_heuristic_iteration_limit`
     - mip_heuristic_maxit
   * - :ref:`option-KNITRO-mip_heuristic_large_neighborhood_search`
     - mip_heuristic_lns
   * - :ref:`option-KNITRO-mip_heuristic_local_search`
     - mip_heuristic_local_search
   * - :ref:`option-KNITRO-mip_heuristic_mpec`
     - mip_heuristic_mpec
   * - :ref:`option-KNITRO-mip_heuristic_strategy`
     - mip_heuristic_strategy
   * - :ref:`option-KNITRO-mip_heuristic_terminate`
     - mip_heuristic_terminate
   * - :ref:`option-KNITRO-mip_implications`
     - mip_implications
   * - :ref:`option-KNITRO-mip_integer_variables_relaxable`
     - mip_relaxable
   * - :ref:`option-KNITRO-mip_integer_variables_strategy`
     - mip_intvar_strategy
   * - :ref:`option-KNITRO-mip_method`
     - mip_method
   * - :ref:`option-KNITRO-mip_misqp_heuristic`
     - mip_heuristic_misqp
   * - :ref:`option-KNITRO-mip_multistart`
     - mip_multistart
   * - :ref:`option-KNITRO-mip_objective_cutoff_value`
     - mip_cutoff
   * - :ref:`option-KNITRO-mip_pseudo_cost_initialization`
     - mip_pseudoinit
   * - :ref:`option-KNITRO-mip_restart`
     - mip_restart
   * - :ref:`option-KNITRO-mip_rounding`
     - mip_rounding
   * - :ref:`option-KNITRO-mip_start_algorithm`
     - mip_rootalg
   * - :ref:`option-KNITRO-mip_terminate`
     - mip_terminate
   * - :ref:`option-KNITRO-node_algorithm`
     - mip_nodealg
   * - :ref:`option-KNITRO-node_selection`
     - mip_selectrule
   * - :ref:`option-KNITRO-node_selection_direction`
     - mip_selectdir
   * - :ref:`option-KNITRO-strong_branching_candidates_limit`
     - mip_strong_candlim
   * - :ref:`option-KNITRO-strong_branching_iteration_limit`
     - mip_strong_maxit
   * - :ref:`option-KNITRO-strong_branching_level`
     - mip_strong_level
   * - :ref:`option-KNITRO-clique_cuts`
     - mip_clique
   * - :ref:`option-KNITRO-flow_cover_cuts`
     - mip_cut_flowcover
   * - :ref:`option-KNITRO-gomory_cuts`
     - mip_gomory
   * - :ref:`option-KNITRO-knapsack_cuts`
     - mip_knapsack
   * - :ref:`option-KNITRO-lift_and_project_cuts`
     - mip_liftproject
   * - :ref:`option-KNITRO-mir_cuts`
     - mip_mir
   * - :ref:`option-KNITRO-probing_cuts`
     - mip_cut_probing
   * - :ref:`option-KNITRO-zero_half_cuts`
     - mip_zerohalf
   * - :ref:`option-KNITRO-multistart`
     - ms_enable
   * - :ref:`option-KNITRO-multistart_deterministic`
     - ms_deterministic
   * - :ref:`option-KNITRO-multistart_initial_points_cluster`
     - ms_initpt_cluster
   * - :ref:`option-KNITRO-multistart_range`
     - ms_startptrange
   * - :ref:`option-KNITRO-multistart_range_unbounded_variable`
     - ms_maxbndrange
   * - :ref:`option-KNITRO-multistart_seed`
     - ms_seed
   * - :ref:`option-KNITRO-multistart_termination_condition`
     - ms_terminate
   * - :ref:`option-KNITRO-number_of_best_solutions`
     - ms_num_to_save
   * - :ref:`option-KNITRO-number_of_multistart_points`
     - ms_maxsolves
   * - :ref:`option-KNITRO-solution_distance`
     - ms_savetol
   * - :ref:`option-KNITRO-number_of_gradient_computation_threads`
     - findiff_numthreads
   * - :ref:`option-KNITRO-number_of_blas_threads`
     - blas_numthreads
   * - :ref:`option-KNITRO-number_of_linear_system_threads`
     - linsolver_numthreads
   * - :ref:`option-KNITRO-number_of_mip_threads`
     - mip_numthreads
   * - :ref:`option-KNITRO-number_of_multistart_threads`
     - ms_numthreads
   * - :ref:`option-KNITRO-number_of_threads`
     - numthreads
   * - :ref:`option-KNITRO-presolve`
     - presolve
   * - :ref:`option-KNITRO-presolve_initial_point`
     - presolve_initpt
   * - :ref:`option-KNITRO-presolve_level`
     - presolve_level
   * - :ref:`option-KNITRO-presolve_passes`
     - presolve_passes
   * - :ref:`option-KNITRO-presolve_redundant_constraints`
     - presolveop_redundant
   * - :ref:`option-KNITRO-presolve_substitution`
     - presolveop_substitution
   * - :ref:`option-KNITRO-presolve_substitution_tolerance`
     - presolveop_substitution_tol
   * - :ref:`option-KNITRO-presolve_tolerance`
     - presolve_tol
   * - :ref:`option-KNITRO-tighten_variable_bounds`
     - presolveop_tighten
   * - :ref:`option-KNITRO-mip_output_level`
     - mip_outinterval
   * - :ref:`option-KNITRO-multi_algorithm_output`
     - ma_outsub
   * - :ref:`option-KNITRO-status_file_display`
     - outlev
   * - :ref:`option-KNITRO-absolute_optimality_tolerance`
     - opttol_abs
   * - :ref:`option-KNITRO-function_evaluations_limit`
     - maxfevals
   * - :ref:`option-KNITRO-infeasibility_tolerance_iteration_limit`
     - infeastol_iters
   * - :ref:`option-KNITRO-multi_algorithm_termination`
     - ma_terminate
   * - :ref:`option-KNITRO-objective_goal`
     - fstopval
   * - :ref:`option-KNITRO-relative_improvement_iterations`
     - ftol_iters
   * - :ref:`option-KNITRO-relative_improvement_tolerance`
     - ftol
   * - :ref:`option-KNITRO-relative_optimality_tolerance`
     - opttol
   * - :ref:`option-KNITRO-absolute_feasibility_tolerance`
     - feastol_abs
   * - :ref:`option-KNITRO-infeasibility_tolerance`
     - infeastol
   * - :ref:`option-KNITRO-lp_feasibility_tolerance`
     - act_lpfeastol
   * - :ref:`option-KNITRO-relative_feasibility_tolerance`
     - feastol
   * - :ref:`option-KNITRO-tuner`
     - tuner
   * - :ref:`option-KNITRO-tuner_output`
     - tuner_outsub
   * - :ref:`option-KNITRO-tuner_terminate`
     - tuner_terminate
   * - :ref:`option-KNITRO-tuner_time_limit`
     - tuner_maxtime_cpu
