
.. _IPOPT_to_AIMMS_Mapping:


IPOPT to AIMMS Mapping
======================

**Description** 

The table shows in the left column the parameters from IPOPT that can be set in AIMMS; the right column displays for each IPOPT parameter the associated AIMMS option.

.. list-table::

   * - **Name in IPOPT**
     - **Option name in AIMMS**
   * - accept_every_trial_step
     - :ref:`option-IPOPT-always_accept_full_trial_step`
   * - acceptable_compl_inf_tol
     - :ref:`option-IPOPT-acceptable_complementarity_tolerance`
   * - acceptable_constr_viol_tol
     - :ref:`option-IPOPT-acceptable_constraint_violation_tolerance`
   * - acceptable_dual_inf_tol
     - :ref:`option-IPOPT-acceptable_dual_infeasibility_tolerance`
   * - acceptable_iter
     - :ref:`option-IPOPT-maximum_number_of_acceptable_iterations`
   * - acceptable_obj_change_tol
     - :ref:`option-IPOPT-acceptable_objective_change_tolerance`
   * - acceptable_tol
     - :ref:`option-IPOPT-acceptable_relative_convergence_tolerance`
   * - alpha_for_y
     - :ref:`option-IPOPT-constraint_multipliers_step_size_method`
   * - alpha_for_y_tol
     - :ref:`option-IPOPT-equality_multipliers_switch_tolerance`
   * - barrier_tol_factor
     - :ref:`option-IPOPT-barrier_convergence_tolerance_factor`
   * - bound_frac
     - :ref:`option-IPOPT-point_to_bound_relative_distance`
   * - bound_mult_init_method
     - :ref:`option-IPOPT-bound_multipliers_initialization_method`
   * - bound_mult_init_val
     - :ref:`option-IPOPT-initial_value_for_bound_multipliers`
   * - bound_mult_reset_threshold
     - :ref:`option-IPOPT-bound_multipliers_reset_threshold`
   * - bound_push
     - :ref:`option-IPOPT-point_to_bound_absolute_distance`
   * - bound_relax_factor
     - :ref:`option-IPOPT-factor_for_initial_bounds_relaxation`
   * - check_derivatives_for_naninf
     - :ref:`option-IPOPT-check_derivatives_for_invalid_numbers`
   * - compl_inf_tol
     - :ref:`option-IPOPT-complementarity_tolerance`
   * - constr_mult_init_max
     - :ref:`option-IPOPT-constraint_multipliers_initial_guess_limit`
   * - constr_mult_reset_threshold
     - :ref:`option-IPOPT-constraint_multipliers_reset_threshold`
   * - constr_viol_tol
     - :ref:`option-IPOPT-constraint_violation_tolerance`
   * - corrector_type
     - :ref:`option-IPOPT-corrector_steps_type`
   * - derivative_test
     - :ref:`option-IPOPT-derivative_testing`
   * - derivative_test_perturbation
     - :ref:`option-IPOPT-derivative_test_perturbation_size`
   * - derivative_test_print_all
     - :ref:`option-IPOPT-derivative_checker_verbosity`
   * - derivative_test_tol
     - :ref:`option-IPOPT-derivative_test_tolerance`
   * - diverging_iterates_tol
     - :ref:`option-IPOPT-diverging_iterates_tolerance`
   * - dual_inf_tol
     - :ref:`option-IPOPT-dual_infeasibility_tolerance`
   * - evaluate_orig_obj_at_resto_trial
     - :ref:`option-IPOPT-use_original_objective_function_in_restoration_phase`
   * - expect_infeasible_problem
     - :ref:`option-IPOPT-quickly_detect_infeasible_problem`
   * - expect_infeasible_problem_ctol
     - :ref:`option-IPOPT-minimum_violation_infeasible_problem`
   * - expect_infeasible_problem_ytol
     - :ref:`option-IPOPT-maximum_multipliers_infeasible_problem`
   * - first_hessian_perturbation
     - :ref:`option-IPOPT-first_hessian_perturbation_size`
   * - fixed_mu_oracle
     - :ref:`option-IPOPT-fixed_mode_oracle`
   * - fixed_variable_treatment
     - :ref:`option-IPOPT-fixed_variable_handling`
   * - hessian_approximation
     - :ref:`option-IPOPT-method_for_hessian_computation`
   * - hessian_constant
     - :ref:`option-IPOPT-assume_quadratic_problem`
   * - honor_original_bounds
     - :ref:`option-IPOPT-honor_original_bounds`
   * - jac_c_constant
     - :ref:`option-IPOPT-assume_equality_constraints_are_linear`
   * - jac_d_constant
     - :ref:`option-IPOPT-assume_inequality_constraints_are_linear`
   * - jacobian_regularization_value
     - :ref:`option-IPOPT-jacobian_regularization_value`
   * - limited_memory_max_history
     - :ref:`option-IPOPT-hessian_approximation_history_memory_limit`
   * - limited_memory_max_skipping
     - :ref:`option-IPOPT-hessian_approximation_successive_iterations_limit`
   * - linear_scaling_on_demand
     - :ref:`option-IPOPT-linear_system_scaling`
   * - linear_solver
     - :ref:`option-IPOPT-linear_solver_selection`
   * - linear_system_scaling
     - :ref:`option-IPOPT-linear_system_scaling_method`
   * - ma27_la_init_factor
     - :ref:`option-IPOPT-ma27_real_workspace_memory`
   * - ma27_liw_init_factor
     - :ref:`option-IPOPT-ma27_integer_workspace_memory`
   * - ma27_meminc_factor
     - :ref:`option-IPOPT-ma27_increment_factor_for_workspace_size`
   * - ma27_pivtol
     - :ref:`option-IPOPT-ma27_pivot_tolerance`
   * - ma27_pivtolmax
     - :ref:`option-IPOPT-ma27_maximum_pivot_tolerance`
   * - ma57_automatic_scaling
     - :ref:`option-IPOPT-ma57_scaling`
   * - ma57_block_size
     - :ref:`option-IPOPT-ma57_block_size`
   * - ma57_node_amalgamation
     - :ref:`option-IPOPT-ma57_node_amalgamation_parameter`
   * - ma57_pivot_order
     - :ref:`option-IPOPT-ma57_pivot_order`
   * - ma57_pivtol
     - :ref:`option-IPOPT-ma57_pivot_tolerance`
   * - ma57_pivtolmax
     - :ref:`option-IPOPT-ma57_maximum_pivot_tolerance`
   * - ma57_pre_alloc
     - :ref:`option-IPOPT-ma57_work_space_memory_safety_factor`
   * - ma57_small_pivot_flag
     - :ref:`option-IPOPT-ma57_small_pivot_parameter`
   * - ma77_u
     - :ref:`option-IPOPT-ma77_pivot_tolerance`
   * - ma77_umax
     - :ref:`option-IPOPT-ma77_maximum_pivot_tolerance`
   * - ma86_u
     - :ref:`option-IPOPT-ma86_pivot_tolerance`
   * - ma86_umax
     - :ref:`option-IPOPT-ma86_maximum_pivot_tolerance`
   * - ma97_u
     - :ref:`option-IPOPT-ma97_pivot_tolerance`
   * - ma97_umax
     - :ref:`option-IPOPT-ma97_maximum_pivot_tolerance`
   * - max_hessian_perturbation
     - :ref:`option-IPOPT-maximum_hessian_perturbation`
   * - max_iter
     - :ref:`option-IPOPT-maximum_number_of_iterations`
   * - max_refinement_steps
     - :ref:`option-IPOPT-maximum_number_of_refinement_steps`
   * - max_soc
     - :ref:`option-IPOPT-second_order_correction_trial_steps_limit`
   * - mehrotra_algorithm
     - :ref:`option-IPOPT-execute_mehrotra_algorithm`
   * - min_hessian_perturbation
     - :ref:`option-IPOPT-minimum_hessian_perturbation`
   * - min_refinement_steps
     - :ref:`option-IPOPT-minimum_number_of_refinement_steps`
   * - mu_init
     - :ref:`option-IPOPT-barrier_parameter_initial_value`
   * - mu_linear_decrease_factor
     - :ref:`option-IPOPT-linear_decrease_factor_barrier_parameter`
   * - mu_max
     - :ref:`option-IPOPT-maximum_value_for_barrier_parameter`
   * - mu_max_fact
     - :ref:`option-IPOPT-adaptive_strategy_factor_limit`
   * - mu_min
     - :ref:`option-IPOPT-minimum_value_for_barrier_parameter`
   * - mu_oracle
     - :ref:`option-IPOPT-adaptive_strategy_oracle`
   * - mu_strategy
     - :ref:`option-IPOPT-barrier_parameter_update_strategy`
   * - mu_superlinear_decrease_power
     - :ref:`option-IPOPT-superlinear_decrease_rate_barrier_parameter`
   * - mumps_mem_percent
     - :ref:`option-IPOPT-mumps_working_space_percentage_increase`
   * - mumps_permuting_scaling
     - :ref:`option-IPOPT-mumps_permuting_and_scaling`
   * - mumps_pivot_order
     - :ref:`option-IPOPT-mumps_pivot_order`
   * - mumps_pivtol
     - :ref:`option-IPOPT-mumps_pivot_tolerance`
   * - mumps_pivtolmax
     - :ref:`option-IPOPT-mumps_maximum_pivot_tolerance`
   * - mumps_scaling
     - :ref:`option-IPOPT-mumps_scaling`
   * - nlp_lower_bound_inf
     - :ref:`option-IPOPT-minus_infinity_lower_bound`
   * - nlp_scaling_max_gradient
     - :ref:`option-IPOPT-maximum_gradient_after_nlp_scaling`
   * - nlp_scaling_method
     - :ref:`option-IPOPT-nlp_scaling_method`
   * - nlp_upper_bound_inf
     - :ref:`option-IPOPT-infinity_upper_bound`
   * - obj_scaling_factor
     - :ref:`option-IPOPT-objective_function_scaling_factor`
   * - perturb_dec_fact
     - :ref:`option-IPOPT-hessian_perturbation_decrease_factor`
   * - perturb_inc_fact
     - :ref:`option-IPOPT-hessian_perturbation_increase_factor`
   * - perturb_inc_fact_first
     - :ref:`option-IPOPT-first_hessian_perturbation_increase_factor`
   * - point_perturbation_radius
     - :ref:`option-IPOPT-maximum_perturbation_of_evaluation_point`
   * - print_level
     - :ref:`option-IPOPT-output_verbosity_level`
   * - print_options_documentation
     - :ref:`option-IPOPT-print_all_available_algorithmic_options`
   * - print_user_options
     - :ref:`option-IPOPT-print_all_user_selected_options`
   * - quality_function_max_section_steps
     - :ref:`option-IPOPT-quality_function_section_steps_limit`
   * - recalc_y
     - :ref:`option-IPOPT-recalculate_constraint_multipliers`
   * - recalc_y_feas_tol
     - :ref:`option-IPOPT-recalculate_constraint_multipliers_tolerance`
   * - required_infeasibility_reduction
     - :ref:`option-IPOPT-required_infeasibility_reduction`
   * - slack_bound_frac
     - :ref:`option-IPOPT-slack_to_bound_relative_distance`
   * - slack_bound_push
     - :ref:`option-IPOPT-slack_to_bound_absolute_distance`
   * - soft_resto_pderror_reduction_factor
     - :ref:`option-IPOPT-reduction_factor_primal_dual_error`
   * - start_with_resto
     - :ref:`option-IPOPT-force_start_in_restoration_phase`
   * - tol
     - :ref:`option-IPOPT-relative_convergence_tolerance`
   * - watchdog_shortened_iter_trigger
     - :ref:`option-IPOPT-watchdog_shortened_iteration_trigger`
   * - watchdog_trial_iter_max
     - :ref:`option-IPOPT-maximum_number_of_watchdog_iterations`

