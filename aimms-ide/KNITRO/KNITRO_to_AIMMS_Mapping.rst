

.. _KNITRO_to_AIMMS_Mapping:


Knitro to AIMMS Mapping
============================

**Description** 

The table shows in the left column the parameters from Knitro that can be set in AIMMS; the right column displays for each Knitro option the associated AIMMS option.
	
.. list-table::

   * - **Name in Knitro**
     - **Option name in AIMMS**
   * - act_lpalg
     - :ref:`option-KNITRO-lp_algorithm`
   * - act_lpfeastol
     - :ref:`option-KNITRO-lp_feasibility_tolerance`
   * - act_lppenalty
     - :ref:`option-KNITRO-objective_reduction`
   * - act_lppresolve
     - :ref:`option-KNITRO-lp_presolve`
   * - act_lpsolver
     - :ref:`option-KNITRO-lp_solver`
   * - act_qpalg
     - :ref:`option-KNITRO-qp_algorithm`
   * - act_qppenalty
     - :ref:`option-KNITRO-act_qppenalty`
   * - bar_conic_enable
     - :ref:`option-KNITRO-barrier_enable_conic`
   * - bar_directinterval
     - :ref:`option-KNITRO-direct_step_interval`
   * - bar_feasible
     - :ref:`option-KNITRO-feasible_mode`
   * - bar_feasmodetol
     - :ref:`option-KNITRO-feasible_mode_activation_tolerance`
   * - bar_globalize
     - :ref:`option-KNITRO-barrier_globalize`
   * - bar_initmu
     - :ref:`option-KNITRO-initial_barrier_parameter_value`
   * - bar_initpi_mpec
     - :ref:`option-KNITRO-initial_barrier_penalty_value_mpec`
   * - bar_initpt
     - :ref:`option-KNITRO-initial_point_strategy`
   * - bar_linsys
     - :ref:`option-KNITRO-linear_system_form_used`
   * - bar_linsys_storage
     - :ref:`option-KNITRO-linear_system_memory_usage`
   * - bar_maxcorrectors
     - :ref:`option-KNITRO-barrier_corrector_steps_limit`
   * - bar_maxcrossit
     - :ref:`option-KNITRO-crossover_iterations_limit`
   * - bar_maxmu
     - :ref:`option-KNITRO-barrier_maximum_mu`
   * - bar_maxrefactor
     - :ref:`option-KNITRO-refactorization_limit`
   * - bar_mpec_heuristic
     - :ref:`option-KNITRO-barrier_mpec_heuristic`
   * - bar_murule
     - :ref:`option-KNITRO-barrier_parameter_strategy`
   * - bar_penaltycons
     - :ref:`option-KNITRO-barrier_penalty_constraint_strategy`
   * - bar_penaltyrule
     - :ref:`option-KNITRO-barrier_penalty_parameter_strategy`
   * - bar_refinement
     - :ref:`option-KNITRO-barrier_refinement`
   * - bar_relaxcons
     - :ref:`option-KNITRO-barrier_relax_constraints`
   * - bar_slackboundpush
     - :ref:`option-KNITRO-barrier_slack_bound_push`
   * - bar_switchobj
     - :ref:`option-KNITRO-barrier_switch_objective`
   * - bar_switchrule
     - :ref:`option-KNITRO-barrier_switch_rule`
   * - bar_watchdog
     - :ref:`option-KNITRO-barrier_watchdog`
   * - blas_numthreads
     - :ref:`option-KNITRO-number_of_blas_threads`
   * - blasoption
     - :ref:`option-KNITRO-blas_option`
   * - cg_maxit
     - :ref:`option-KNITRO-conjugate_gradient_iteration_limit`
   * - cg_pmem
     - :ref:`option-KNITRO-conjugate_gradient_memory_limit`
   * - cg_precond
     - :ref:`option-KNITRO-conjugate_gradient_preconditioner`
   * - cg_stoptol
     - :ref:`option-KNITRO-conjugate_gradient_stopping_tolerance`
   * - convex
     - :ref:`option-KNITRO-mark_as_convex`
   * - datacheck
     - :ref:`option-KNITRO-data_check`
   * - debug
     - :ref:`option-KNITRO-debugging_output`
   * - delta
     - :ref:`option-KNITRO-initial_trust_scaling_factor`
   * - feastol
     - :ref:`option-KNITRO-relative_feasibility_tolerance`
   * - feastol_abs
     - :ref:`option-KNITRO-absolute_feasibility_tolerance`
   * - findiff_estnoise
     - :ref:`option-KNITRO-estimate_noise_in_the_model`
   * - findiff_numthreads
     - :ref:`option-KNITRO-number_of_gradient_computation_threads`
   * - fstopval
     - :ref:`option-KNITRO-objective_goal`
   * - ftol
     - :ref:`option-KNITRO-relative_improvement_tolerance`
   * - ftol_iters
     - :ref:`option-KNITRO-relative_improvement_iterations`
   * - gradopt
     - :ref:`option-KNITRO-gradient_computation_method`
   * - hessopt
     - :ref:`option-KNITRO-hessian_computation_method`
   * - honorbnds
     - :ref:`option-KNITRO-honor_bounds`
   * - infeastol
     - :ref:`option-KNITRO-infeasibility_tolerance`
   * - infeastol_iters
     - :ref:`option-KNITRO-infeasibility_tolerance_iteration_limit`
   * - initpenalty
     - :ref:`option-KNITRO-initial_penalty_value`
   * - linesearch
     - :ref:`option-KNITRO-linesearch_strategy`
   * - linesearch_maxtrials
     - :ref:`option-KNITRO-linesearch_trials_limit`
   * - linsolver
     - :ref:`option-KNITRO-linear_solver`
   * - linsolver_maxitref
     - :ref:`option-KNITRO-linear_system_max_iterative_refinements`
   * - linsolver_nodeamalg
     - :ref:`option-KNITRO-linear_solver_node_amalgamation`
   * - linsolver_numthreads
     - :ref:`option-KNITRO-number_of_linear_system_threads`
   * - linsolver_ooc
     - :ref:`option-KNITRO-linear_solver_out_of_core`
   * - linsolver_ordering
     - :ref:`option-KNITRO-linear_solver_ordering`
   * - linsolver_pivottol
     - :ref:`option-KNITRO-initial_pivot_treshold`
   * - linsolver_scaling
     - :ref:`option-KNITRO-linear_solver_scaling`
   * - lmsize
     - :ref:`option-KNITRO-limited_memory_size`
   * - ma_outsub
     - :ref:`option-KNITRO-multi_algorithm_output`
   * - ma_terminate
     - :ref:`option-KNITRO-multi_algorithm_termination`
   * - maxfevals
     - :ref:`option-KNITRO-function_evaluations_limit`
   * - maxit
     - :ref:`option-AIMMS-iteration_limit`  in 'Solvers general'
   * - maxtime_cpu
     - :ref:`option-AIMMS-time_limit`  in 'Solvers general'
   * - mip_branchrule
     - :ref:`option-KNITRO-mip_branching_rule`
   * - mip_clique
     - :ref:`option-KNITRO-clique_cuts`
   * - mip_cut_flowcover
     - :ref:`option-KNITRO-flow_cover_cuts`
   * - mip_cut_probing
     - :ref:`option-KNITRO-probing_cuts`
   * - mip_cutoff
     - :ref:`option-KNITRO-mip_objective_cutoff_value`
   * - mip_debug
     - :ref:`option-KNITRO-debugging_mip_output`
   * - mip_gomory
     - :ref:`option-KNITRO-gomory_cuts`
   * - mip_gub_branch
     - :ref:`option-KNITRO-mip_gub_branch`
   * - mip_heuristic
     - :ref:`option-KNITRO-mip_heuristic`
   * - mip_heuristic_diving
     - :ref:`option-KNITRO-mip_heuristic_diving`
   * - mip_heuristic_feaspump
     - :ref:`option-KNITRO-mip_heuristic_feasibility_pump`
   * - mip_heuristic_lns
     - :ref:`option-KNITRO-mip_heuristic_large_neighborhood_search`
   * - mip_heuristic_localsearch
     - :ref:`option-KNITRO-mip_heuristic_local_search`
   * - mip_heuristic_maxit
     - :ref:`option-KNITRO-mip_heuristic_iteration_limit`
   * - mip_heuristic_misqp
     - :ref:`option-KNITRO-mip_misqp_heuristic`
   * - mip_heuristic_mpec
     - :ref:`option-KNITRO-mip_heuristic_mpec`
   * - mip_heuristic_strategy
     - :ref:`option-KNITRO-mip_heuristic_strategy`
   * - mip_heuristic_terminate
     - :ref:`option-KNITRO-mip_heuristic_terminate`
   * - mip_implications
     - :ref:`option-KNITRO-mip_implications`
   * - mip_integer_tol
     - :ref:`option-KNITRO-integrality`
   * - mip_intvar_strategy
     - :ref:`option-KNITRO-mip_integer_variables_strategy`
   * - mip_knapsack
     - :ref:`option-KNITRO-knapsack_cuts`
   * - mip_liftproject
     - :ref:`option-KNITRO-lift_and_project_cuts`
   * - mip_lpalg
     - :ref:`option-KNITRO-mip_algorithm`
   * - mip_maxnodes
     - :ref:`option-KNITRO-maximal_number_of_nodes`
   * - mip_maxsolves
     - :ref:`option-KNITRO-maximal_number_of_subproblem_solves`
   * - mip_method
     - :ref:`option-KNITRO-mip_method`
   * - mip_mir
     - :ref:`option-KNITRO-mir_cuts`
   * - mip_multistart
     - :ref:`option-KNITRO-mip_multistart`
   * - mip_nodealg
     - :ref:`option-KNITRO-node_algorithm`
   * - mip_numthreads
     - :ref:`option-KNITRO-number_of_mip_threads`
   * - mip_outinterval
     - :ref:`option-KNITRO-mip_output_level`
   * - mip_pseudoinit
     - :ref:`option-KNITRO-mip_pseudo_cost_initialization`
   * - mip_relaxable
     - :ref:`option-KNITRO-mip_integer_variables_relaxable`
   * - mip_restart
     - :ref:`option-KNITRO-mip_restart`
   * - mip_rootalg
     - :ref:`option-KNITRO-mip_start_algorithm`
   * - mip_rounding
     - :ref:`option-KNITRO-mip_rounding`
   * - mip_selectdir
     - :ref:`option-KNITRO-node_selection_direction`
   * - mip_selectrule
     - :ref:`option-KNITRO-node_selection`
   * - mip_strong_candlim
     - :ref:`option-KNITRO-strong_branching_candidates_limit`
   * - mip_strong_level
     - :ref:`option-KNITRO-strong_branching_level`
   * - mip_strong_maxit
     - :ref:`option-KNITRO-strong_branching_iteration_limit`
   * - mip_terminate
     - :ref:`option-KNITRO-mip_terminate`
   * - mip_zerohalf
     - :ref:`option-KNITRO-zero_half_cuts`
   * - ms_deterministic
     - :ref:`option-KNITRO-multistart_deterministic`
   * - ms_enable
     - :ref:`option-KNITRO-multistart`
   * - ms_intpt_cluster
     - :ref:`option-KNITRO-multistart_initial_points_cluster`
   * - ms_maxbndrange
     - :ref:`option-KNITRO-multistart_range_unbounded_variable`
   * - ms_maxsolves
     - :ref:`option-KNITRO-number_of_multistart_points`
   * - ms_num_to_save
     - :ref:`option-KNITRO-number_of_best_solutions`
   * - ms_numthreads
     - :ref:`option-KNITRO-number_of_multistart_threads`
   * - ms_savetol
     - :ref:`option-KNITRO-solution_distance`
   * - ms_seed
     - :ref:`option-KNITRO-multistart_seed`
   * - ms_startptrange
     - :ref:`option-KNITRO-multistart_range`
   * - ms_terminate
     - :ref:`option-KNITRO-multistart_termination_condition`
   * - ncvx_qcqp_init
     - :ref:`option-KNITRO-qp_and_qcqp_initialization_strategy`
   * - numthreads
     - :ref:`option-KNITRO-number_of_threads`
   * - objrange
     - :ref:`option-KNITRO-unboundedness_range`
   * - opttol
     - :ref:`option-KNITRO-relative_optimality_tolerance`
   * - opttol_abs
     - :ref:`option-KNITRO-absolute_optimality_tolerance`
   * - outlev
     - :ref:`option-KNITRO-status_file_display`
   * - numthreads
     - :ref:`option-KNITRO-number_of_threads`
   * - presolve
     - :ref:`option-KNITRO-presolve`
   * - presolve_initpt
     - :ref:`option-KNITRO-presolve_initial_point`
   * - presolve_level
     - :ref:`option-KNITRO-presolve_level`
   * - presolve_passes
     - :ref:`option-KNITRO-presolve_passes`
   * - presolve_tol
     - :ref:`option-KNITRO-presolve_tolerance`
   * - presolveop_redundant
     - :ref:`option-KNITRO-presolve_redundant_constraints`
   * - presolveop_substitution
     - :ref:`option-KNITRO-presolve_substitution`
   * - presolveop_substitution_tol
     - :ref:`option-KNITRO-presolve_substitution_tolerance`
   * - presolveop_tighten
     - :ref:`option-KNITRO-tighten_variable_bounds`
   * - restarts
     - :ref:`option-KNITRO-restarts`
   * - restarts_maxit
     - :ref:`option-KNITRO-restarts_iteration_limit`
   * - scale
     - :ref:`option-KNITRO-scaling`
   * - scale_vars
     - :ref:`option-KNITRO-scale_variables`
   * - soc
     - :ref:`option-KNITRO-second_order_correction`
   * - strat_warm_start
     - :ref:`option-KNITRO-warm_start_strategy`
   * - tuner
     - :ref:`option-KNITRO-tuner`
   * - tuner_maxtime_cpu
     - :ref:`option-KNITRO-tuner_time_limit`
   * - tuner_outsub
     - :ref:`option-KNITRO-tuner_output`
   * - tuner_terminate
     - :ref:`option-KNITRO-tuner_terminate`
   * - xtol
     - :ref:`option-KNITRO-solution_progress_tolerance`
   * - xtol_iters
     - :ref:`option-KNITRO-solution_progress_iterations`
