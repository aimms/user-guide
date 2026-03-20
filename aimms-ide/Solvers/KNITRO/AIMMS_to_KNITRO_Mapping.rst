

.. _AIMMS_to_KNITRO_Mapping:


AIMMS to Knitro Mapping
============================

**Description** 

The table shows in the left column the AIMMS Knitro options; the right column displays for the AIMMS option the Knitro option that is associated with it.

.. list-table::

   * - **Option name in AIMMS**
     - **Name in Knitro**
   * - :ref:`Advanced - Estimate Noise in the Model <option-KNITRO-estimate_noise_in_the_model>`
     - findiff_estnoise
   * - :ref:`Advanced - Gradient Computation Method <option-KNITRO-gradient_computation_method>`
     - gradopt
   * - :ref:`Advanced - Initial Penalty Value <option-KNITRO-initial_penalty_value>`
     - initpenalty
   * - :ref:`Advanced - Initial Pivot Treshold <option-KNITRO-initial_pivot_treshold>`
     - linsolver_pivottol
   * - :ref:`Advanced - Initial Trust Scaling Factor <option-KNITRO-initial_trust_scaling_factor>`
     - delta
   * - :ref:`Advanced - Linesearch Strategy <option-KNITRO-linesearch_strategy>`
     - linesearch
   * - :ref:`Advanced - Linesearch Trials Limit <option-KNITRO-linesearch_trials_limit>`
     - linesearch_maxtrials
   * - :ref:`Advanced - LP Algorithm <option-KNITRO-lp_algorithm>`
     - act_lpalg
   * - :ref:`Advanced - Objective Reduction <option-KNITRO-objective_reduction>`
     - act_lppenalty
   * - :ref:`Advanced - LP Presolve <option-KNITRO-lp_presolve>`
     - act_lppresolve
   * - :ref:`Advanced - QP and QCQP Initialization Strategy <option-KNITRO-qp_and_qcqp_initialization_strategy>`
     - ncvx_qcqp_init
   * - :ref:`Advanced - Solution Progress Iterations <option-KNITRO-solution_progress_iterations>`
     - xtol_iters
   * - :ref:`Advanced - Solution Progress Tolerance <option-KNITRO-solution_progress_tolerance>`
     - xtol
   * - :ref:`Debugging - Data Check <option-KNITRO-data_check>`
     - datacheck
   * - :ref:`Debugging - Debugging MIP output <option-KNITRO-debugging_mip_output>`
     - mip_debug
   * - :ref:`Debugging - Debugging Output <option-KNITRO-debugging_output>`
     - debug
   * - :ref:`General - Act QPpenalty <option-KNITRO-act_qppenalty>`
     - act_qppenalty
   * - :ref:`General - Algorithm <option-KNITRO-algorithm>`
     - algorithm
   * - :ref:`General - BLAS Option <option-KNITRO-blas_option>`
     - blasoption
   * - :ref:`General - Honor Bounds <option-KNITRO-honor_bounds>`
     - honorbnds
   * - :ref:`General - Linear Solver <option-KNITRO-linear_solver>`
     - linsolver
   * - :ref:`General - Linear Solver Node Amalgamation <option-KNITRO-linear_solver_node_amalgamation>`
     - linsolver_nodeamalg
   * - :ref:`General - Linear Solver Ordering <option-KNITRO-linear_solver_ordering>`
     - linsolver_ordering
   * - :ref:`General - Linear Solver Out of Core <option-KNITRO-linear_solver_out_of_core>`
     - linsolver_ooc
   * - :ref:`General - Linear Solver Scaling <option-KNITRO-linear_solver_scaling>`
     - linsolver_scaling
   * - :ref:`General - Linear System Max Iterative Refinements <option-KNITRO-linear_system_max_iterative_refinements>`
     - linsolver_maxitref
   * - :ref:`General - LP Solver <option-KNITRO-lp_solver>`
     - act_lpsolver
   * - :ref:`General - Mark as Convex <option-KNITRO-mark_as_convex>`
     - convex
   * - :ref:`General - QP Algorithm <option-KNITRO-qp_algorithm>`
     - act_qpalg
   * - :ref:`General - Restarts <option-KNITRO-restarts>`
     - restarts
   * - :ref:`General - Restarts Iteration Limit <option-KNITRO-restarts_iteration_limit>`
     - restarts_maxit
   * - :ref:`General - Scale Variables <option-KNITRO-scale_variables>`
     - scale_vars
   * - :ref:`General - Scaling <option-KNITRO-scaling>`
     - scale
   * - :ref:`General - Unboundedness Range <option-KNITRO-unboundedness_range>`
     - objrange
   * - :ref:`General - Warm Start Strategy <option-KNITRO-warm_start_strategy>`
     - strat_warm_start
   * - :ref:`Hessian - Hessian Computation Method <option-KNITRO-hessian_computation_method>`
     - hessopt
   * - :ref:`Hessian - Limited Memory Size <option-KNITRO-limited_memory_size>`
     - lmsize
   * - :ref:`Hessian - Second Order Correction <option-KNITRO-second_order_correction>`
     - soc
   * - :ref:`Interior Point - Barrier Corrector Steps Limit <option-KNITRO-barrier_corrector_steps_limit>`
     - bar_maxcorrectors
   * - :ref:`Interior Point - Barrier Enable Conic <option-KNITRO-barrier_enable_conic>`
     - bar_conic_enable
   * - :ref:`Interior Point - Barrier Globalize <option-KNITRO-barrier_globalize>`
     - bar_globalize
   * - :ref:`Interior Point - Barrier Maximum Mu <option-KNITRO-barrier_maximum_mu>`
     - bar_maxmu
   * - :ref:`Interior Point - Barrier MPEC Heuristic <option-KNITRO-barrier_mpec_heuristic>`
     - bar_mpec_heuristic
   * - :ref:`Interior Point - Barrier Parameter Strategy <option-KNITRO-barrier_parameter_strategy>`
     - bar_murule
   * - :ref:`Interior Point - Barrier Penalty Constraint Strategy <option-KNITRO-barrier_penalty_constraint_strategy>`
     - bar_penaltycons
   * - :ref:`Interior Point - Barrier Penalty Parameter Strategy <option-KNITRO-barrier_penalty_parameter_strategy>`
     - bar_penaltyrule
   * - :ref:`Interior Point - Barrier Refinement <option-KNITRO-barrier_refinement>`
     - bar_refinement
   * - :ref:`Interior Point - Barrier Relax Constraints <option-KNITRO-barrier_relax_constraints>`
     - bar_relaxcons
   * - :ref:`Interior Point - Barrier Slack Bound Push <option-KNITRO-barrier_slack_bound_push>`
     - bar_slackboundpush
   * - :ref:`Interior Point - Barrier Switch Objective <option-KNITRO-barrier_switch_objective>`
     - bar_switchobj
   * - :ref:`Interior Point - Barrier Switch Rule <option-KNITRO-barrier_switch_rule>`
     - bar_switchrule
   * - :ref:`Interior Point - Barrier Watchdog <option-KNITRO-barrier_watchdog>`
     - bar_watchdog
   * - :ref:`Interior Point - Conjugate Gradient Iteration Limit <option-KNITRO-conjugate_gradient_iteration_limit>`
     - cg_maxit
   * - :ref:`Interior Point - Conjugate Gradient Memory Limit <option-KNITRO-conjugate_gradient_memory_limit>`
     - cg_pmem
   * - :ref:`Interior Point - Conjugate Gradient Preconditioner <option-KNITRO-conjugate_gradient_preconditioner>`
     - cg_precond
   * - :ref:`Interior Point - Conjugate Gradient Stopping Tolerance <option-KNITRO-conjugate_gradient_stopping_tolerance>`
     - cg_stoptol
   * - :ref:`Interior Point - Crossover Iterations Limit <option-KNITRO-crossover_iterations_limit>`
     - bar_maxcrossit
   * - :ref:`Interior Point - Direct Step Interval <option-KNITRO-direct_step_interval>`
     - bar_directinterval
   * - :ref:`Interior Point - Feasible Mode <option-KNITRO-feasible_mode>`
     - bar_feasible
   * - :ref:`Interior Point - Feasible Mode Activation Tolerance <option-KNITRO-feasible_mode_activation_tolerance>`
     - bar_feasmodetol
   * - :ref:`Interior Point - Initial Barrier Parameter Value <option-KNITRO-initial_barrier_parameter_value>`
     - bar_initmu
   * - :ref:`Interior Point - Initial Barrier Penalty Value MPEC <option-KNITRO-initial_barrier_penalty_value_mpec>`
     - bar_initpi_mpec
   * - :ref:`Interior Point - Initial Point Strategy <option-KNITRO-initial_point_strategy>`
     - bar_initpt
   * - :ref:`Interior Point - Linear System Form Used <option-KNITRO-linear_system_form_used>`
     - bar_linsys
   * - :ref:`Interior Point - Linear System Memory Usage <option-KNITRO-linear_system_memory_usage>`
     - bar_linsys_storage
   * - :ref:`Interior Point - Refactorization Limit <option-KNITRO-refactorization_limit>`
     - bar_maxrefactor
   * - :ref:`MIP - Integrality <option-KNITRO-integrality>`
     - mip_integer_tol
   * - :ref:`MIP - Maximal Number of Nodes <option-KNITRO-maximal_number_of_nodes>`
     - mip_maxnodes
   * - :ref:`MIP - Maximal Number of Subproblem Solves <option-KNITRO-maximal_number_of_subproblem_solves>`
     - mip_maxsolves
   * - :ref:`MIP - MIP Algorithm <option-KNITRO-mip_algorithm>`
     - mip_lpalg
   * - :ref:`MIP - MIP Branching Rule <option-KNITRO-mip_branching_rule>`
     - mip_branchrule
   * - :ref:`MIP - MIP GUB Branch <option-KNITRO-mip_gub_branch>`
     - mip_gub_branch
   * - :ref:`MIP - MIP Heuristic <option-KNITRO-mip_heuristic>`
     - mip_heuristic
   * - :ref:`MIP - MIP Heuristic Diving <option-KNITRO-mip_heuristic_diving>`
     - mip_heuristic_diving
   * - :ref:`MIP - MIP Heuristic Feasibility Pump <option-KNITRO-mip_heuristic_feasibility_pump>`
     - mip_heuristic_feaspump
   * - :ref:`MIP - MIP Heuristic Iteration Limit <option-KNITRO-mip_heuristic_iteration_limit>`
     - mip_heuristic_maxit
   * - :ref:`MIP - MIP Heuristic Large Neighborhood Search <option-KNITRO-mip_heuristic_large_neighborhood_search>`
     - mip_heuristic_lns
   * - :ref:`MIP - MIP Heuristic Local Search <option-KNITRO-mip_heuristic_local_search>`
     - mip_heuristic_local_search
   * - :ref:`MIP - MIP Heuristic MPEC <option-KNITRO-mip_heuristic_mpec>`
     - mip_heuristic_mpec
   * - :ref:`MIP - MIP Heuristic Strategy <option-KNITRO-mip_heuristic_strategy>`
     - mip_heuristic_strategy
   * - :ref:`MIP - MIP Heuristic Terminate <option-KNITRO-mip_heuristic_terminate>`
     - mip_heuristic_terminate
   * - :ref:`MIP - MIP Implications <option-KNITRO-mip_implications>`
     - mip_implications
   * - :ref:`MIP - MIP Integer Variables Relaxable <option-KNITRO-mip_integer_variables_relaxable>`
     - mip_relaxable
   * - :ref:`MIP - MIP Integer Variables Strategy <option-KNITRO-mip_integer_variables_strategy>`
     - mip_intvar_strategy
   * - :ref:`MIP - MIP Method <option-KNITRO-mip_method>`
     - mip_method
   * - :ref:`MIP - MIP MISQP Heuristic <option-KNITRO-mip_misqp_heuristic>`
     - mip_heuristic_misqp
   * - :ref:`MIP - MIP Multistart <option-KNITRO-mip_multistart>`
     - mip_multistart
   * - :ref:`MIP - MIP Objective Cutoff Value <option-KNITRO-mip_objective_cutoff_value>`
     - mip_cutoff
   * - :ref:`MIP - MIP Pseudo Cost Initialization <option-KNITRO-mip_pseudo_cost_initialization>`
     - mip_pseudoinit
   * - :ref:`MIP - MIP Restart <option-KNITRO-mip_restart>`
     - mip_restart
   * - :ref:`MIP - MIP Rounding <option-KNITRO-mip_rounding>`
     - mip_rounding
   * - :ref:`MIP - MIP Start Algorithm <option-KNITRO-mip_start_algorithm>`
     - mip_rootalg
   * - :ref:`MIP - MIP Terminate <option-KNITRO-mip_terminate>`
     - mip_terminate
   * - :ref:`MIP - Node Algorithm <option-KNITRO-node_algorithm>`
     - mip_nodealg
   * - :ref:`MIP - Node Selection <option-KNITRO-node_selection>`
     - mip_selectrule
   * - :ref:`MIP - Node Selection_Direction <option-KNITRO-node_selection_direction>`
     - mip_selectdir
   * - :ref:`MIP - Strong Branching Candidates Limit <option-KNITRO-strong_branching_candidates_limit>`
     - mip_strong_candlim
   * - :ref:`MIP - Strong Branching Iteration Limit <option-KNITRO-strong_branching_iteration_limit>`
     - mip_strong_maxit
   * - :ref:`MIP - Strong Branching Level <option-KNITRO-strong_branching_level>`
     - mip_strong_level
   * - :ref:`MIP Cuts - Clique Cuts <option-KNITRO-clique_cuts>`
     - mip_clique
   * - :ref:`MIP Cuts - Flow Cover Cuts <option-KNITRO-flow_cover_cuts>`
     - mip_cut_flowcover
   * - :ref:`MIP Cuts - Gomory Cuts <option-KNITRO-gomory_cuts>`
     - mip_gomory
   * - :ref:`MIP Cuts - Knapsack Cuts <option-KNITRO-knapsack_cuts>`
     - mip_knapsack
   * - :ref:`MIP Cuts - Lift and Project Cuts <option-KNITRO-lift_and_project_cuts>`
     - mip_liftproject
   * - :ref:`MIP Cuts - MIR Cuts <option-KNITRO-mir_cuts>`
     - mip_mir
   * - :ref:`MIP Cuts - Probing Cuts <option-KNITRO-probing_cuts>`
     - mip_cut_probing
   * - :ref:`MIP Cuts - Zero Half Cuts <option-KNITRO-zero_half_cuts>`
     - mip_zerohalf
   * - :ref:`Multistart - Multistart <option-KNITRO-multistart>`
     - ms_enable
   * - :ref:`Multistart - Multistart Deterministic <option-KNITRO-multistart_deterministic>`
     - ms_deterministic
   * - :ref:`Multistart - Multistart Initial Points Cluster <option-KNITRO-multistart_initial_points_cluster>`
     - ms_initpt_cluster
   * - :ref:`Multistart - Multistart Range <option-KNITRO-multistart_range>`
     - ms_startptrange
   * - :ref:`Multistart - Multistart Range Unbounded Variable <option-KNITRO-multistart_range_unbounded_variable>`
     - ms_maxbndrange
   * - :ref:`Multistart - Multistart Seed <option-KNITRO-multistart_seed>`
     - ms_seed
   * - :ref:`Multistart - Multistart Termination Condition <option-KNITRO-multistart_termination_condition>`
     - ms_terminate
   * - :ref:`Multistart - Number of Best Solutions <option-KNITRO-number_of_best_solutions>`
     - ms_num_to_save
   * - :ref:`Multistart - Number of Multistart Points <option-KNITRO-number_of_multistart_points>`
     - ms_maxsolves
   * - :ref:`Multistart - Solution Distance <option-KNITRO-solution_distance>`
     - ms_savetol
   * - :ref:`Parallel - Number of Gradient Computation Threads <option-KNITRO-number_of_gradient_computation_threads>`
     - findiff_numthreads
   * - :ref:`Parallel - Number of BLAS Threads <option-KNITRO-number_of_blas_threads>`
     - blas_numthreads
   * - :ref:`Parallel - Number of Linear System Threads <option-KNITRO-number_of_linear_system_threads>`
     - linsolver_numthreads
   * - :ref:`Parallel - Number of MIP Threads <option-KNITRO-number_of_mip_threads>`
     - mip_numthreads
   * - :ref:`Parallel - Number of Multistart Threads <option-KNITRO-number_of_multistart_threads>`
     - ms_numthreads
   * - :ref:`Parallel - Number of Threads <option-KNITRO-number_of_threads>`
     - numthreads
   * - :ref:`Presolve - Presolve <option-KNITRO-presolve>`
     - presolve
   * - :ref:`Presolve - Presolve Initial Point <option-KNITRO-presolve_initial_point>`
     - presolve_initpt
   * - :ref:`Presolve - Presolve Level <option-KNITRO-presolve_level>`
     - presolve_level
   * - :ref:`Presolve - Presolve Passes <option-KNITRO-presolve_passes>`
     - presolve_passes
   * - :ref:`Presolve - Presolve Redundant Constraints <option-KNITRO-presolve_redundant_constraints>`
     - presolveop_redundant
   * - :ref:`Presolve - Presolve Substitution <option-KNITRO-presolve_substitution>`
     - presolveop_substitution
   * - :ref:`Presolve - Presolve Substitution Tolerance <option-KNITRO-presolve_substitution_tolerance>`
     - presolveop_substitution_tol
   * - :ref:`Presolve - Presolve Tolerance <option-KNITRO-presolve_tolerance>`
     - presolve_tol
   * - :ref:`Presolve - Tighten Variable Bounds <option-KNITRO-tighten_variable_bounds>`
     - presolveop_tighten
   * - :ref:`Reporting - MIP Output Level <option-KNITRO-mip_output_level>`
     - mip_outinterval
   * - :ref:`Reporting - Multi Algorithm Output <option-KNITRO-multi_algorithm_output>`
     - ma_outsub
   * - :ref:`Reporting - Status File Display <option-KNITRO-status_file_display>`
     - outlev
   * - :ref:`Termination - Absolute Optimality Tolerance <option-KNITRO-absolute_optimality_tolerance>`
     - opttol_abs
   * - :ref:`Termination - Function Evaluations Limit <option-KNITRO-function_evaluations_limit>`
     - maxfevals
   * - :ref:`Termination - Infeasibility Tolerance Iteration Limit <option-KNITRO-infeasibility_tolerance_iteration_limit>`
     - infeastol_iters
   * - :ref:`Termination - Multi Algorithm Termination <option-KNITRO-multi_algorithm_termination>`
     - ma_terminate
   * - :ref:`Termination - Objective Goal <option-KNITRO-objective_goal>`
     - fstopval
   * - :ref:`Termination - Relative Improvement Iterations <option-KNITRO-relative_improvement_iterations>`
     - ftol_iters
   * - :ref:`Termination - Relative Improvement Tolerance <option-KNITRO-relative_improvement_tolerance>`
     - ftol
   * - :ref:`Termination - Relative Optimality Tolerance <option-KNITRO-relative_optimality_tolerance>`
     - opttol
   * - :ref:`Tolerances - Absolute Feasibility Tolerance <option-KNITRO-absolute_feasibility_tolerance>`
     - feastol_abs
   * - :ref:`Tolerances - Infeasibility Tolerance <option-KNITRO-infeasibility_tolerance>`
     - infeastol
   * - :ref:`Tolerances - LP Feasibility Tolerance <option-KNITRO-lp_feasibility_tolerance>`
     - act_lpfeastol
   * - :ref:`Tolerances - Relative Feasibility Tolerance <option-KNITRO-relative_feasibility_tolerance>`
     - feastol
   * - :ref:`Tuner - Tuner <option-KNITRO-tuner>`
     - tuner
   * - :ref:`Tuner - Tuner Output <option-KNITRO-tuner_output>`
     - tuner_outsub
   * - :ref:`Tuner - Tuner Terminate <option-KNITRO-tuner_terminate>`
     - tuner_terminate
   * - :ref:`Tuner - Tuner Time Limit <option-KNITRO-tuner_time_limit>`
     - tuner_maxtime_cpu
