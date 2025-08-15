.. _IPOPT_to_AIMMS_Mapping:


IPOPT to AIMMS Mapping
======================

**Description** 

The table shows in the left column the parameters from IPOPT that can be set in AIMMS; the right column displays for each IPOPT parameter the associated AIMMS option.

.. list-table::

   * - **Name in IPOPT**
     - **Option name in AIMMS**
   * - accept_every_trial_step
     - :ref:`IPOPT_Line_search_-_Always_accept_full_trial_step`
   * - acceptable_compl_inf_tol
     - :ref:`IPOPT_Termination_-_Acceptable_complementarity_tolerance`
   * - acceptable_constr_viol_tol
     - :ref:`IPOPT_Termination_-_Acceptable_constraint_violation_tolerance`
   * - acceptable_dual_inf_tol
     - :ref:`IPOPT_Termination_-_Acceptable_dual_infeasibility_tolerance`
   * - acceptable_iter
     - :ref:`IPOPT_Termination_-_Maximum_number_of_acceptable_iterations`
   * - acceptable_obj_change_tol
     - :ref:`IPOPT_Termination_-_Acceptable_objective_change_tolerance`
   * - acceptable_tol
     - :ref:`IPOPT_Termination_-_Acceptable_relative_convergence_tolerance`
   * - alpha_for_y
     - :ref:`IPOPT_Multipliers_-_Constraint_multipliers_step_size_method`
   * - alpha_for_y_tol
     - :ref:`IPOPT_Multipliers_-_Equality_multipliers_switch_tolerance`
   * - barrier_tol_factor
     - :ref:`IPOPT_Barrier_-_Barrier_convergence_tolerance_factor`
   * - bound_frac
     - :ref:`IPOPT_Initialization_-_Point_to_bound_relative_distance`
   * - bound_mult_init_method
     - :ref:`IPOPT_Initialization_-_Bound_multipliers_initialization_method`
   * - bound_mult_init_val
     - :ref:`IPOPT_Initialization_-_Initial_value_for_bound_multipliers`
   * - bound_mult_reset_threshold
     - :ref:`IPOPT_Restoration_phase_-_Bound_multipliers_reset_threshold`
   * - bound_push
     - :ref:`IPOPT_Initialization_-_Point_to_bound_absolute_distance`
   * - bound_relax_factor
     - :ref:`IPOPT_NLP_-_Factor_for_initial_bounds_relaxation`
   * - check_derivatives_for_naninf
     - :ref:`IPOPT_NLP_-_Check_derivatives_for_invalid_numbers`
   * - compl_inf_tol
     - :ref:`IPOPT_Termination_-_Complementarity_tolerance`
   * - constr_mult_init_max
     - :ref:`IPOPT_Initialization_-_Constraint_multipliers_initial_guess_limit`
   * - constr_mult_reset_threshold
     - :ref:`IPOPT_Restoration_phase_-_Constraint_multipliers_reset_threshold`
   * - constr_viol_tol
     - :ref:`IPOPT_Termination_-_Constraint_violation_tolerance`
   * - corrector_type
     - :ref:`IPOPT_Line_search_-_Corrector_steps_type`
   * - derivative_test
     - :ref:`IPOPT_Derivative_test_-_Derivative_testing`
   * - derivative_test_perturbation
     - :ref:`IPOPT_Derivative_test_-_Derivative_test_perturbation_size`
   * - derivative_test_print_all
     - :ref:`IPOPT_Derivative_test_-_Derivative_checker_verbosity`
   * - derivative_test_tol
     - :ref:`IPOPT_Derivative_test_-_Derivative_test_tolerance`
   * - diverging_iterates_tol
     - :ref:`IPOPT_Termination_-_Diverging_iterates_tolerance`
   * - dual_inf_tol
     - :ref:`IPOPT_Termination_-_Dual_infeasibility_tolerance`
   * - evaluate_orig_obj_at_resto_trial
     - :ref:`IPOPT_Restoration_phase_-_Use_original_objective_function_in_restoration_phase`
   * - expect_infeasible_problem
     - :ref:`IPOPT_Restoration_phase_-_Quickly_detect_infeasible_problem`
   * - expect_infeasible_problem_ctol
     - :ref:`IPOPT_Restoration_phase_-_Minimum_violation_infeasible_problem`
   * - expect_infeasible_problem_ytol
     - :ref:`IPOPT_Restoration_phase_-_Maximum_multipliers_infeasible_problem`
   * - first_hessian_perturbation
     - :ref:`IPOPT_Hessian_perturbation_-_First_Hessian_perturbation_size`
   * - fixed_mu_oracle
     - :ref:`IPOPT_Barrier_-_Fixed_mode_oracle`
   * - fixed_variable_treatment
     - :ref:`IPOPT_NLP_-_Fixed_variable_handling`
   * - hessian_approximation
     - :ref:`IPOPT_Quasi-Newton_-_Method_for_Hessian_computation`
   * - hessian_constant
     - :ref:`IPOPT_NLP_-_Assume_quadratic_problem`
   * - honor_original_bounds
     - :ref:`IPOPT_NLP_-_Honor_original_bounds`
   * - jac_c_constant
     - :ref:`IPOPT_NLP_-_Assume_equality_constraints_are_linear`
   * - jac_d_constant
     - :ref:`IPOPT_NLP_-_Assume_inequality_constraints_are_linear`
   * - jacobian_regularization_value
     - :ref:`IPOPT_Hessian_perturbation_-_Jacobian_regularization_value`
   * - limited_memory_max_history
     - :ref:`IPOPT_Quasi-Newton_-_Hessian_approximation_history_memory_limit`
   * - limited_memory_max_skipping
     - :ref:`IPOPT_Quasi-Newton_-_Hessian_approximation_successive_iterations_limit`
   * - linear_scaling_on_demand
     - :ref:`IPOPT_Linear_solver_-_Linear_system_scaling`
   * - linear_solver
     - :ref:`IPOPT_Linear_solver_-_Linear_solver_selection`
   * - linear_system_scaling
     - :ref:`IPOPT_Linear_solver_-_Linear_system_scaling_method`
   * - ma27_la_init_factor
     - :ref:`IPOPT_Linear_solver_-_MA27_real_workspace_memory`
   * - ma27_liw_init_factor
     - :ref:`IPOPT_Linear_solver_-_MA27_integer_workspace_memory`
   * - ma27_meminc_factor
     - :ref:`IPOPT_Linear_solver_-_MA27_increment_factor_for_workspace_size`
   * - ma27_pivtol
     - :ref:`IPOPT_Linear_solver_-_MA27_pivot_tolerance`
   * - ma27_pivtolmax
     - :ref:`IPOPT_Linear_solver_-_MA27_maximum_pivot_tolerance`
   * - ma57_automatic_scaling
     - :ref:`IPOPT_Linear_solver_-_MA57_scaling`
   * - ma57_block_size
     - :ref:`IPOPT_Linear_solver_-_MA57_block_size`
   * - ma57_node_amalgamation
     - :ref:`IPOPT_Linear_solver_-_MA57_node_amalgamation_paramet`
   * - ma57_pivot_order
     - :ref:`IPOPT_Linear_solver_-_MA57_pivot_order`
   * - ma57_pivtol
     - :ref:`IPOPT_Linear_solver_-_MA57_pivot_tolerance`
   * - ma57_pivtolmax
     - :ref:`IPOPT_Linear_solver_-_MA57_maximum_pivot_tolerance`
   * - ma57_pre_alloc
     - :ref:`IPOPT_Linear_solver_-_MA57_work_space_memory_safety_f`
   * - ma57_small_pivot_flag
     - :ref:`IPOPT_Linear_solver_-_MA57_small_pivot_parameter`
   * - ma77_u
     - :ref:`IPOPT_Linear_solver_-_MA77_pivot_tolerance`
   * - ma77_umax
     - :ref:`IPOPT_Linear_solver_-_MA77_maximum_pivot_tolerance`
   * - ma86_u
     - :ref:`IPOPT_Linear_solver_-_MA86_pivot_tolerance`
   * - ma86_umax
     - :ref:`IPOPT_Linear_solver_-_MA86_maximum_pivot_tolerance`
   * - ma97_u
     - :ref:`IPOPT_Linear_solver_-_MA97_pivot_tolerance`
   * - ma97_umax
     - :ref:`IPOPT_Linear_solver_-_MA97_maximum_pivot_tolerance`
   * - max_hessian_perturbation
     - :ref:`IPOPT_Hessian_perturbation_-_Maximum_Hessian_perturbation`
   * - max_iter
     - :ref:`IPOPT_Termination_-_Maximum_number_of_iterations`
   * - max_refinement_steps
     - :ref:`IPOPT_Linear_solver_-_Maximum_number_of_refinement_steps`
   * - max_soc
     - :ref:`IPOPT_Line_search_-_Second_order_correction_trial_steps_limit`
   * - mehrotra_algorithm
     - :ref:`IPOPT_Barrier_-_Execute_Mehrotra_algorithm`
   * - min_hessian_perturbation
     - :ref:`IPOPT_Hessian_perturbation_-_Minimum_Hessian_perturbation`
   * - min_refinement_steps
     - :ref:`IPOPT_Linear_solver_-_Minimum_number_of_refinement_steps`
   * - mu_init
     - :ref:`IPOPT_Barrier_-_Barrier_parameter_initial_value`
   * - mu_linear_decrease_factor
     - :ref:`IPOPT_Barrier_-_Linear_decrease_factor_barrier_parameter`
   * - mu_max
     - :ref:`IPOPT_Barrier_-_Maximum_value_for_barrier_parameter`
   * - mu_max_fact
     - :ref:`IPOPT_Barrier_-_Adaptive_strategy_factor_limit`
   * - mu_min
     - :ref:`IPOPT_Barrier_-_Minimum_value_for_barrier_parameter`
   * - mu_oracle
     - :ref:`IPOPT_Barrier_-_Adaptive_strategy_oracle`
   * - mu_strategy
     - :ref:`IPOPT_Barrier_-_Barrier_parameter_update_strategy`
   * - mu_superlinear_decrease_power
     - :ref:`IPOPT_Barrier_-_Superlinear_decrease_rate_barrier_parameter`
   * - mumps_mem_percent
     - :ref:`IPOPT_Linear_solver_-_MUMPS_working_space_percentage_increase`
   * - mumps_permuting_scaling
     - :ref:`IPOPT_Linear_solver_-_MUMPS_permuting_and_scaling`
   * - mumps_pivot_order
     - :ref:`IPOPT_Linear_solver_-_MUMPS_pivot_order`
   * - mumps_pivtol
     - :ref:`IPOPT_Linear_solver_-_MUMPS_pivot_tolerance`
   * - mumps_pivtolmax
     - :ref:`IPOPT_Linear_solver_-_MUMPS_maximum_pivot_tolerance`
   * - mumps_scaling
     - :ref:`IPOPT_Linear_solver_-_MUMPS_scaling`
   * - nlp_lower_bound_inf
     - :ref:`IPOPT_NLP_-_Minus_infinity_lower_bound`
   * - nlp_scaling_max_gradient
     - :ref:`IPOPT_NLP_scaling_-_Maximum_gradient_after_NLP_scaling`
   * - nlp_scaling_method
     - :ref:`IPOPT_NLP_scaling_-_NLP_scaling_method`
   * - nlp_upper_bound_inf
     - :ref:`IPOPT_NLP_-_Infinity_upper_bound`
   * - obj_scaling_factor
     - :ref:`IPOPT_NLP_scaling_-_Objective_function_scaling_factor`
   * - perturb_dec_fact
     - :ref:`IPOPT_Hessian_perturbation_-_Hessian_perturbation_decrease_factor`
   * - perturb_inc_fact
     - :ref:`IPOPT_Hessian_perturbation_-_Hessian_perturbation_increase_factor`
   * - perturb_inc_fact_first
     - :ref:`IPOPT_Hessian_perturbation_-_First_Hessian_perturbation_increase_factor`
   * - point_perturbation_radius
     - :ref:`IPOPT_Derivative_test_-_Maximum_perturbation_of_evaluation_point`
   * - print_level
     - :ref:`IPOPT_Output_-_Output_verbosity_level`
   * - print_options_documentation
     - :ref:`IPOPT_Output_-_Print_all_available_algorithmic_options`
   * - print_user_options
     - :ref:`IPOPT_Output_-_Print_all_user_selected_options`
   * - quality_function_max_section_steps
     - :ref:`IPOPT_Barrier_-_Quality_function_section_steps_limit`
   * - recalc_y
     - :ref:`IPOPT_Multipliers_-_Recalculate_constraint_multipliers`
   * - recalc_y_feas_tol
     - :ref:`IPOPT_Multipliers_-_Recalculate_constraint_multipliers_tolerance`
   * - required_infeasibility_reduction
     - :ref:`IPOPT_Restoration_phase_-_Required_infeasibility_reduction`
   * - slack_bound_frac
     - :ref:`IPOPT_Initialization_-_Slack_to_bound_relative_distance`
   * - slack_bound_push
     - :ref:`IPOPT_Initialization_-_Slack_to_bound_absolute_distance`
   * - soft_resto_pderror_reduction_factor
     - :ref:`IPOPT_Restoration_phase_-_Reduction_factor_primal_dual_error`
   * - start_with_resto
     - :ref:`IPOPT_Restoration_phase_-_Force_start_in_restoration_phase`
   * - tol
     - :ref:`IPOPT_Termination_-_Relative_convergence_tolerance`
   * - watchdog_shortened_iter_trigger
     - :ref:`IPOPT_Line_search_-_Watchdog_shortened_iteration_trigger`
   * - watchdog_trial_iter_max
     - :ref:`IPOPT_Line_search_-_Maximum_number_of_watchdog_iterations`

