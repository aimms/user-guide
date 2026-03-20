

.. _AIMMS_to_IPOPT_Mapping:


AIMMS to IPOPT Mapping
======================

**Description** 

The table shows in the left column the AIMMS IPOPT options while the right column displays the associated IPOPT parameter.

.. list-table::

   * - **Option name in AIMMS** 
     - **Name in IPOPT** 
   * - :doc:`Barrier Parameter - Adaptive Strategy Factor Limit <Barrier parameter/IPOPT_Barrier_-_Adaptive_strategy_factor_limit>` 
     - mu_max_fact
   * - :doc:`Barrier Parameter - Adaptive Strategy Oracle <Barrier parameter/IPOPT_Barrier_-_Adaptive_strategy_oracle>` 
     - mu_oracle
   * - :doc:`Barrier Parameter - Barrier Convergence Tolerance Factor <Barrier parameter/IPOPT_Barrier_-_Barrier_convergence_tolerance_factor>` 
     - barrier_tol_factor
   * - :doc:`Barrier Parameter - Barrier Parameter Initial Value <Barrier parameter/IPOPT_Barrier_-_Barrier_parameter_initial_value>` 
     - mu_init
   * - :doc:`Barrier Parameter - Barrier Parameter Update Strategy <Barrier parameter/IPOPT_Barrier_-_Barrier_parameter_update_strategy>` 
     - mu_strategy
   * - :doc:`Barrier Parameter - Execute Mehrotra Algorithm <Barrier parameter/IPOPT_Barrier_-_Execute_Mehrotra_algorithm>` 
     - mehrotra_algorithm
   * - :doc:`Barrier Parameter - Fixed Mode Oracle <Barrier parameter/IPOPT_Barrier_-_Fixed_mode_oracle>` 
     - fixed_mu_oracle
   * - :doc:`Barrier Parameter - Linear Decrease Factor Barrier Parameter <Barrier parameter/IPOPT_Barrier_-_Linear_decrease_factor_barrier_parameter>` 
     - mu_linear_decrease_factor
   * - :doc:`Barrier Parameter - Maximum Value for Barrier Parameter <Barrier parameter/IPOPT_Barrier_-_Maximum_value_for_barrier_parameter>` 
     - mu_max
   * - :doc:`Barrier Parameter - Minimum Value for Barrier Parameter <Barrier parameter/IPOPT_Barrier_-_Minimum_value_for_barrier_parameter>` 
     - mu_min
   * - :doc:`Barrier Parameter - Quality Function Section Steps Limit <Barrier parameter/IPOPT_Barrier_-_Quality_function_section_steps_limit>` 
     - quality_function_max_section_steps
   * - :doc:`Barrier Parameter - Superlinear Decrease Rate Barrier Parameter <Barrier parameter/IPOPT_Barrier_-_Superlinear_decrease_rate_barrier_parameter>` 
     - mu_superlinear_decrease_power
   * - :doc:`Derivative Test - Derivative Checker Verbosity <Derivative test/IPOPT_Derivative_test_-_Derivative_checker_verbosity>` 
     - derivative_test_print_all
   * - :doc:`Derivative Test - Derivative Test Perturbation Size <Derivative test/IPOPT_Derivative_test_-_Derivative_test_perturbation_size>` 
     - derivative_test_perturbation
   * - :doc:`Derivative Test - Derivative Test Tolerance <Derivative test/IPOPT_Derivative_test_-_Derivative_test_tolerance>` 
     - derivative_test_tol
   * - :doc:`Derivative Test - Derivative Testing <Derivative test/IPOPT_Derivative_test_-_Derivative_testing>` 
     - derivative_test
   * - :doc:`Derivative Test - Maximum Perturbation of Evaluation Point <Derivative test/IPOPT_Derivative_test_-_Maximum_perturbation_of_evaluation_point>` 
     - point_perturbation_radius
   * - :doc:`Hessian Perturbation - First Hessian Perturbation Increase Factor <Hessian perturbation/IPOPT_Hessian_perturbation_-_First_Hessian_perturbation_increase_factor>` 
     - perturb_inc_fact_first
   * - :doc:`Hessian Perturbation - First Hessian Perturbation Size <Hessian perturbation/IPOPT_Hessian_perturbation_-_First_Hessian_perturbation_size>` 
     - first_hessian_perturbation
   * - :doc:`Hessian Perturbation - Hessian Perturbation Decrease Factor <Hessian perturbation/IPOPT_Hessian_perturbation_-_Hessian_perturbation_decrease_factor>` 
     - perturb_dec_fact
   * - :doc:`Hessian Perturbation - Hessian Perturbation Increase Factor <Hessian perturbation/IPOPT_Hessian_perturbation_-_Hessian_perturbation_increase_factor>` 
     - perturb_inc_fact
   * - :doc:`Hessian Perturbation - Jacobian Regularization Value <Hessian perturbation/IPOPT_Hessian_perturbation_-_Jacobian_regularization_value>` 
     - jacobian_regularization_value
   * - :doc:`Hessian Perturbation - Maximum Hessian Perturbation <Hessian perturbation/IPOPT_Hessian_perturbation_-_Maximum_Hessian_perturbation>` 
     - max_hessian_perturbation
   * - :doc:`Hessian Perturbation - Minimum Hessian Perturbation <Hessian perturbation/IPOPT_Hessian_perturbation_-_Minimum_Hessian_perturbation>` 
     - min_hessian_perturbation
   * - :doc:`Initialization - Bound Multipliers Initialization Method <Initialization/IPOPT_Initialization_-_Bound_multipliers_initialization_method>` 
     - bound_mult_init_method
   * - :doc:`Initialization - Constraint Multipliers Initial Guess Limit <Initialization/IPOPT_Initialization_-_Constraint_multipliers_initial_guess_limit>` 
     - constr_mult_init_max
   * - :doc:`Initialization - Initial Value for Bound Multipliers <Initialization/IPOPT_Initialization_-_Initial_value_for_bound_multipliers>` 
     - bound_mult_init_val
   * - :doc:`Initialization - Point to Bound Absolute Distance <Initialization/IPOPT_Initialization_-_Point_to_bound_absolute_distance>` 
     - bound_push
   * - :doc:`Initialization - Point to Bound Relative Distance <Initialization/IPOPT_Initialization_-_Point_to_bound_relative_distance>` 
     - bound_frac
   * - :doc:`Initialization - Slack to Bound Absolute Distance <Initialization/IPOPT_Initialization_-_Slack_to_bound_absolute_distance>` 
     - slack_bound_push
   * - :doc:`Initialization - Slack to Bound Relative Distance <Initialization/IPOPT_Initialization_-_Slack_to_bound_relative_distance>` 
     - slack_bound_frac
   * - :doc:`Line Search - Always Accept Full Trial Step <Line search/IPOPT_Line_search_-_Always_accept_full_trial_step>` 
     - accept_every_trial_step
   * - :doc:`Line Search - Corrector Steps Type <Line search/IPOPT_Line_search_-_Corrector_steps_type>` 
     - corrector_type
   * - :doc:`Line Search - Maximum Number of Watchdog Iterations <Line search/IPOPT_Line_search_-_Maximum_number_of_watchdog_iterations>` 
     - watchdog_trial_iter_max
   * - :doc:`Line Search - Second Order Correction Trial Steps Limit <Line search/IPOPT_Line_search_-_Second_order_correction_trial_steps_limit>` 
     - max_soc
   * - :doc:`Line Search - Watchdog Shortened Iteration Trigger <Line search/IPOPT_Line_search_-_Watchdog_shortened_iteration_trigger>` 
     - watchdog_shortened_iter_trigger
   * - :doc:`Linear Solver - Linear Solver Selection <Linear solver/IPOPT_Linear_solver_-_Linear_solver_selection>` 
     - linear_solver
   * - :doc:`Linear Solver - Linear System Scaling <Linear solver/IPOPT_Linear_solver_-_Linear_system_scaling>` 
     - linear_scaling_on_demand
   * - :doc:`Linear Solver - Linear System Scaling Method <Linear solver/IPOPT_Linear_solver_-_Linear_system_scaling_method>` 
     - linear_system_scaling
   * - :doc:`Linear Solver - MA27 Increment Factor for Workspace Size <Linear solver/IPOPT_Linear_solver_-_MA27_increment_factor_for_workspace_size>` 
     - ma27_meminc_factor
   * - :doc:`Linear Solver - MA27 Integer Workspace Memory <Linear solver/IPOPT_Linear_solver_-_MA27_integer_workspace_memory>` 
     - ma27_liw_init_factor
   * - :doc:`Linear Solver - MA27 Maximum Pivot Tolerance <Linear solver/IPOPT_Linear_solver_-_MA27_maximum_pivot_tolerance>` 
     - ma27_pivtolmax
   * - :doc:`Linear Solver - MA27 Pivot Tolerance <Linear solver/IPOPT_Linear_solver_-_MA27_pivot_tolerance>` 
     - ma27_pivtol
   * - :doc:`Linear Solver - MA27 Real Workspace Memory <Linear solver/IPOPT_Linear_solver_-_MA27_real_workspace_memory>` 
     - ma27_la_init_factor
   * - :doc:`Linear Solver - MA57 Block Size <Linear solver/IPOPT_Linear_solver_-_MA57_block_size>` 
     - ma57_block_size
   * - :doc:`Linear Solver - MA57 Maximum Pivot Tolerance <Linear solver/IPOPT_Linear_solver_-_MA57_maximum_pivot_tolerance>` 
     - ma57_pivtolmax
   * - :doc:`Linear Solver - MA57 Node Amalgamation Parameter <Linear solver/IPOPT_Linear_solver_-_MA57_node_amalgamation_paramet>` 
     - ma57_node_amalgamation
   * - :doc:`Linear Solver - MA57 Pivot Order <Linear solver/IPOPT_Linear_solver_-_MA57_pivot_order>` 
     - ma57_pivot_order
   * - :doc:`Linear Solver - MA57 Pivot Tolerance <Linear solver/IPOPT_Linear_solver_-_MA57_pivot_tolerance>` 
     - ma57_pivtol
   * - :doc:`Linear Solver - MA57 Scaling <Linear solver/IPOPT_Linear_solver_-_MA57_scaling>` 
     - ma57_automatic_scaling
   * - :doc:`Linear Solver - MA57 Small Pivot Parameter <Linear solver/IPOPT_Linear_solver_-_MA57_small_pivot_parameter>` 
     - ma57_small_pivot_flag
   * - :doc:`Linear Solver - MA57 Work Space Memory Safety Factor <Linear solver/IPOPT_Linear_solver_-_MA57_work_space_memory_safety_f>` 
     - ma57_pre_alloc
   * - :doc:`Linear Solver - MA77 Maximum Pivot Tolerance <Linear solver/IPOPT_Linear_solver_-_MA77_maximum_pivot_tolerance>` 
     - ma77_umax
   * - :doc:`Linear Solver - MA77 Pivot Tolerance <Linear solver/IPOPT_Linear_solver_-_MA77_pivot_tolerance>` 
     - ma77_u
   * - :doc:`Linear Solver - MA86 Maximum Pivot Tolerance <Linear solver/IPOPT_Linear_solver_-_MA86_maximum_pivot_tolerance>` 
     - ma86_umax
   * - :doc:`Linear Solver - MA86 Pivot Tolerance <Linear solver/IPOPT_Linear_solver_-_MA86_pivot_tolerance>` 
     - ma86_u
   * - :doc:`Linear Solver - MA97 Maximum Pivot Tolerance <Linear solver/IPOPT_Linear_solver_-_MA97_maximum_pivot_tolerance>` 
     - ma97_umax
   * - :doc:`Linear Solver - MA97 Pivot Tolerance <Linear solver/IPOPT_Linear_solver_-_MA97_pivot_tolerance>` 
     - ma97_u
   * - :doc:`Linear Solver - Maximum Number of Refinement Steps <Linear solver/IPOPT_Linear_solver_-_Maximum_number_of_refinement_steps>` 
     - max_refinement_steps
   * - :doc:`Linear Solver - Minimum Number of Refinement Steps <Linear solver/IPOPT_Linear_solver_-_Minimum_number_of_refinement_steps>` 
     - min_refinement_steps
   * - :doc:`Linear Solver - MUMPS Maximum Pivot Tolerance <Linear solver/IPOPT_Linear_solver_-_MUMPS_maximum_pivot_tolerance>` 
     - mumps_pivtolmax
   * - :doc:`Linear Solver - MUMPS Permuting and Scaling <Linear solver/IPOPT_Linear_solver_-_MUMPS_permuting_and_scaling>` 
     - mumps_permuting_scaling
   * - :doc:`Linear Solver - MUMPS Pivot Order <Linear solver/IPOPT_Linear_solver_-_MUMPS_pivot_order>` 
     - mumps_pivot_order
   * - :doc:`Linear Solver - MUMPS Pivot Tolerance <Linear solver/IPOPT_Linear_solver_-_MUMPS_pivot_tolerance>` 
     - mumps_pivtol
   * - :doc:`Linear Solver - MUMPS Scaling <Linear solver/IPOPT_Linear_solver_-_MUMPS_scaling>` 
     - mumps_scaling
   * - :doc:`Linear Solver - MUMPS Working Space Percentage Increase <Linear solver/IPOPT_Linear_solver_-_MUMPS_working_space_percentage_increase>` 
     - mumps_mem_percent
   * - :doc:`Multipliers - Constraint Multipliers Step Size Method <Multipliers/IPOPT_Multipliers_-_Constraint_multipliers_step_size_method>` 
     - alpha_for_y
   * - :doc:`Multipliers - Equality Multipliers Switch Tolerance <Multipliers/IPOPT_Multipliers_-_Equality_multipliers_switch_tolerance>` 
     - alpha_for_y_tol
   * - :doc:`Multipliers - Recalculate Constraint Multipliers <Multipliers/IPOPT_Multipliers_-_Recalculate_constraint_multipliers>` 
     - recalc_y
   * - :doc:`Multipliers - Recalculate Constraint Multipliers Tolerance <Multipliers/IPOPT_Multipliers_-_Recalculate_constraint_multipliers_tolerance>` 
     - recalc_y_feas_tol
   * - :doc:`NLP - Assume Equality Constraints Are Linear <NLP/IPOPT_NLP_-_Assume_equality_constraints_are_linear>` 
     - jac_c_constant
   * - :doc:`NLP - Assume Inequality Constraints Are Linear <NLP/IPOPT_NLP_-_Assume_inequality_constraints_are_linear>` 
     - jac_d_constant
   * - :doc:`NLP - Assume Quadratic Problem <NLP/IPOPT_NLP_-_Assume_quadratic_problem>` 
     - hessian_constant
   * - :doc:`NLP - Check Derivatives for Invalid Numbers <NLP/IPOPT_NLP_-_Check_derivatives_for_invalid_numbers>` 
     - check_derivatives_for_naninf
   * - :doc:`NLP - Factor for Initial Bounds Relaxation <NLP/IPOPT_NLP_-_Factor_for_initial_bounds_relaxation>` 
     - bound_relax_factor
   * - :doc:`NLP - Fixed Variable Handling <NLP/IPOPT_NLP_-_Fixed_variable_handling>` 
     - fixed_variable_treatment
   * - :doc:`NLP - Honor Original Bounds <NLP/IPOPT_NLP_-_Honor_original_bounds>` 
     - honor_original_bounds
   * - :doc:`NLP - Infinity Upper Bound <NLP/IPOPT_NLP_-_Infinity_upper_bound>` 
     - nlp_upper_bound_inf
   * - :doc:`NLP - Minus Infinity Lower Bound <NLP/IPOPT_NLP_-_Minus_infinity_lower_bound>` 
     - nlp_lower_bound_inf
   * - :doc:`NLP Scaling - Maximum Gradient after NLP Scaling <NLP scaling/IPOPT_NLP_scaling_-_Maximum_gradient_after_NLP_scaling>` 
     - nlp_scaling_max_gradient
   * - :doc:`NLP Scaling - NLP Scaling Method <NLP scaling/IPOPT_NLP_scaling_-_NLP_scaling_method>` 
     - nlp_scaling_method
   * - :doc:`NLP Scaling - Objective Function Scaling Factor <NLP scaling/IPOPT_NLP_scaling_-_Objective_function_scaling_factor>` 
     - obj_scaling_factor
   * - :doc:`Output - Output Verbosity Level <Output/IPOPT_Output_-_Output_verbosity_level>` 
     - print_level
   * - :doc:`Output - Print All Available Algorithmic Options <Output/IPOPT_Output_-_Print_all_available_algorithmic_options>` 
     - print_options_documentation
   * - :doc:`Output - Print All User Selected Options <Output/IPOPT_Output_-_Print_all_user_selected_options>` 
     - print_user_options
   * - :doc:`Output - Status File <Output/IPOPT_Output_-_Status_file>` 
     - 
   * - :doc:`Quasi-Newton - Hessian Approximation History Memory Limit <Quasi-Newton/IPOPT_Quasi-Newton_-_Hessian_approximation_history_memory_limit>` 
     - limited_memory_max_history
   * - :doc:`Quasi-Newton - Hessian Approximation Successive Iterations Limit <Quasi-Newton/IPOPT_Quasi-Newton_-_Hessian_approximation_successive_iterations_limit>` 
     - limited_memory_max_skipping
   * - :doc:`Quasi-Newton - Method for Hessian Computation <Quasi-Newton/IPOPT_Quasi-Newton_-_Method_for_Hessian_computation>` 
     - hessian_approximation
   * - :doc:`Restoration Phase - Bound Multipliers Reset Threshold <Restoration phase/IPOPT_Restoration_phase_-_Bound_multipliers_reset_threshold>` 
     - bound_mult_reset_threshold
   * - :doc:`Restoration Phase - Constraint Multipliers Reset Threshold <Restoration phase/IPOPT_Restoration_phase_-_Constraint_multipliers_reset_threshold>` 
     - constr_mult_reset_threshold
   * - :doc:`Restoration Phase - Force Start in Restoration Phase <Restoration phase/IPOPT_Restoration_phase_-_Force_start_in_restoration_phase>` 
     - start_with_resto
   * - :doc:`Restoration Phase - Maximum Multipliers Infeasible Problem <Restoration phase/IPOPT_Restoration_phase_-_Maximum_multipliers_infeasible_problem>` 
     - expect_infeasible_problem_ytol
   * - :doc:`Restoration Phase - Minimum Violation Infeasible Problem <Restoration phase/IPOPT_Restoration_phase_-_Minimum_violation_infeasible_problem>` 
     - expect_infeasible_problem_ctol
   * - :doc:`Restoration Phase - Quickly Detect Infeasible Problem <Restoration phase/IPOPT_Restoration_phase_-_Quickly_detect_infeasible_problem>` 
     - expect_infeasible_problem
   * - :doc:`Restoration Phase - Reduction Factor Primal Dual Error <Restoration phase/IPOPT_Restoration_phase_-_Reduction_factor_primal_dual_error>` 
     - soft_resto_pderror_reduction_factor
   * - :doc:`Restoration Phase - Required Infeasibility Reduction <Restoration phase/IPOPT_Restoration_phase_-_Required_infeasibility_reduction>` 
     - required_infeasibility_reduction
   * - :doc:`Restoration Phase - Use Original Objective Function in Restoration Phase <Restoration phase/IPOPT_Restoration_phase_-_Use_original_objective_function_in_restoration_phase>` 
     - evaluate_orig_obj_at_resto_trial
   * - :doc:`Termination - Acceptable Complementarity Tolerance <Termination/IPOPT_Termination_-_Acceptable_complementarity_tolerance>` 
     - acceptable_compl_inf_tol
   * - :doc:`Termination - Acceptable Constraint Violation Tolerance <Termination/IPOPT_Termination_-_Acceptable_constraint_violation_tolerance>` 
     - acceptable_constr_viol_tol
   * - :doc:`Termination - Acceptable Dual Infeasibility Tolerance <Termination/IPOPT_Termination_-_Acceptable_dual_infeasibility_tolerance>` 
     - acceptable_dual_inf_tol
   * - :doc:`Termination - Acceptable Objective Change Tolerance <Termination/IPOPT_Termination_-_Acceptable_objective_change_tolerance>` 
     - acceptable_obj_change_tol
   * - :doc:`Termination - Acceptable Relative Convergence Tolerance <Termination/IPOPT_Termination_-_Acceptable_relative_convergence_tolerance>` 
     - acceptable_tol
   * - :doc:`Termination - Complementarity Tolerance <Termination/IPOPT_Termination_-_Complementarity_tolerance>` 
     - compl_inf_tol
   * - :doc:`Termination - Constraint Violation Tolerance <Termination/IPOPT_Termination_-_Constraint_violation_tolerance>` 
     - constr_viol_tol
   * - :doc:`Termination - Diverging Iterates Tolerance <Termination/IPOPT_Termination_-_Diverging_iterates_tolerance>` 
     - diverging_iterates_tol
   * - :doc:`Termination - Dual Infeasibility Tolerance <Termination/IPOPT_Termination_-_Dual_infeasibility_tolerance>` 
     - dual_inf_tol
   * - :doc:`Termination - Maximum Number of Acceptable Iterations <Termination/IPOPT_Termination_-_Maximum_number_of_acceptable_iterations>` 
     - acceptable_iter
   * - :doc:`Termination - Maximum Number of Iterations <Termination/IPOPT_Termination_-_Maximum_number_of_iterations>` 
     - max_iter
   * - :doc:`Termination - Relative Convergence Tolerance <Termination/IPOPT_Termination_-_Relative_convergence_tolerance>` 
     - tol
