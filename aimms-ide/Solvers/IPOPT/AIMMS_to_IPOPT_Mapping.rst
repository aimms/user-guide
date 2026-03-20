

.. _AIMMS_to_IPOPT_Mapping:


AIMMS to IPOPT Mapping
======================

**Description** 

The table shows in the left column the AIMMS IPOPT options while the right column displays the associated IPOPT parameter.

.. list-table::

   * - **Option name in AIMMS** 
     - **Name in IPOPT** 
   * - :ref:`Barrier parameter - Adaptive strategy factor limit <option-IPOPT-adaptive_strategy_factor_limit>` 
     - mu_max_fact
   * - :ref:`Barrier parameter - Adaptive strategy oracle <option-IPOPT-adaptive_strategy_oracle>` 
     - mu_oracle
   * - :ref:`Barrier parameter - Barrier convergence tolerance factor <option-IPOPT-barrier_convergence_tolerance_factor>` 
     - barrier_tol_factor
   * - :ref:`Barrier parameter - Barrier parameter initial value <option-IPOPT-barrier_parameter_initial_value>` 
     - mu_init
   * - :ref:`Barrier parameter - Barrier parameter update strategy <option-IPOPT-barrier_parameter_update_strategy>` 
     - mu_strategy
   * - :ref:`Barrier parameter - Execute Mehrotra algorithm <option-IPOPT-execute_mehrotra_algorithm>` 
     - mehrotra_algorithm
   * - :ref:`Barrier parameter - Fixed mode oracle <option-IPOPT-fixed_mode_oracle>` 
     - fixed_mu_oracle
   * - :ref:`Barrier parameter - Linear decrease factor barrier parameter <option-IPOPT-linear_decrease_factor_barrier_parameter>` 
     - mu_linear_decrease_factor
   * - :ref:`Barrier parameter - Maximum value for barrier parameter <option-IPOPT-maximum_value_for_barrier_parameter>` 
     - mu_max
   * - :ref:`Barrier parameter - Minimum value for barrier parameter <option-IPOPT-minimum_value_for_barrier_parameter>` 
     - mu_min
   * - :ref:`Barrier parameter - Quality function section steps limit <option-IPOPT-quality_function_section_steps_limit>` 
     - quality_function_max_section_steps
   * - :ref:`Barrier parameter - Superlinear decrease rate barrier parameter <option-IPOPT-superlinear_decrease_rate_barrier_parameter>` 
     - mu_superlinear_decrease_power
   * - :ref:`Derivative test - Derivative checker verbosity <option-IPOPT-derivative_checker_verbosity>` 
     - derivative_test_print_all
   * - :ref:`Derivative test - Derivative test perturbation size <option-IPOPT-derivative_test_perturbation_size>` 
     - derivative_test_perturbation
   * - :ref:`Derivative test - Derivative test tolerance <option-IPOPT-derivative_test_tolerance>` 
     - derivative_test_tol
   * - :ref:`Derivative test - Derivative testing <option-IPOPT-derivative_testing>` 
     - derivative_test
   * - :ref:`Derivative test - Maximum perturbation of evaluation point <option-IPOPT-maximum_perturbation_of_evaluation_point>` 
     - point_perturbation_radius
   * - :ref:`Hessian perturbation - First Hessian perturbation increase factor <option-IPOPT-first_hessian_perturbation_increase_factor>` 
     - perturb_inc_fact_first
   * - :ref:`Hessian perturbation - First Hessian perturbation size <option-IPOPT-first_hessian_perturbation_size>` 
     - first_hessian_perturbation
   * - :ref:`Hessian perturbation - Hessian perturbation decrease factor <option-IPOPT-hessian_perturbation_decrease_factor>` 
     - perturb_dec_fact
   * - :ref:`Hessian perturbation - Hessian perturbation increase factor <option-IPOPT-hessian_perturbation_increase_factor>` 
     - perturb_inc_fact
   * - :ref:`Hessian perturbation - Jacobian regularization value <option-IPOPT-jacobian_regularization_value>` 
     - jacobian_regularization_value
   * - :ref:`Hessian perturbation - Maximum Hessian perturbation <option-IPOPT-maximum_hessian_perturbation>` 
     - max_hessian_perturbation
   * - :ref:`Hessian perturbation - Minimum Hessian perturbation <option-IPOPT-minimum_hessian_perturbation>` 
     - min_hessian_perturbation
   * - :ref:`Initialization - Bound multipliers initialization method <option-IPOPT-bound_multipliers_initialization_method>` 
     - bound_mult_init_method
   * - :ref:`Initialization - Constraint multipliers initial guess limit <option-IPOPT-constraint_multipliers_initial_guess_limit>` 
     - constr_mult_init_max
   * - :ref:`Initialization - Initial value for bound multipliers <option-IPOPT-initial_value_for_bound_multipliers>` 
     - bound_mult_init_val
   * - :ref:`Initialization - Point to bound absolute distance <option-IPOPT-point_to_bound_absolute_distance>` 
     - bound_push
   * - :ref:`Initialization - Point to bound relative distance <option-IPOPT-point_to_bound_relative_distance>` 
     - bound_frac
   * - :ref:`Initialization - Slack to bound absolute distance <option-IPOPT-slack_to_bound_absolute_distance>` 
     - slack_bound_push
   * - :ref:`Initialization - Slack to bound relative distance <option-IPOPT-slack_to_bound_relative_distance>` 
     - slack_bound_frac
   * - :ref:`Line search - Always accept full trial step <option-IPOPT-always_accept_full_trial_step>` 
     - accept_every_trial_step
   * - :ref:`Line search - Corrector steps type <option-IPOPT-corrector_steps_type>` 
     - corrector_type
   * - :ref:`Line search - Maximum number of watchdog iterations <option-IPOPT-maximum_number_of_watchdog_iterations>` 
     - watchdog_trial_iter_max
   * - :ref:`Line search - Second order correction trial steps limit <option-IPOPT-second_order_correction_trial_steps_limit>` 
     - max_soc
   * - :ref:`Line search - Watchdog shortened iteration trigger <option-IPOPT-watchdog_shortened_iteration_trigger>` 
     - watchdog_shortened_iter_trigger
   * - :ref:`Linear solver - Linear solver selection <option-IPOPT-linear_solver_selection>` 
     - linear_solver
   * - :ref:`Linear solver - Linear system scaling <option-IPOPT-linear_system_scaling>` 
     - linear_scaling_on_demand
   * - :ref:`Linear solver - Linear system scaling method <option-IPOPT-linear_system_scaling_method>` 
     - linear_system_scaling
   * - :ref:`Linear solver - MA27 increment factor for workspace size <option-IPOPT-ma27_increment_factor_for_workspace_size>` 
     - ma27_meminc_factor
   * - :ref:`Linear solver - MA27 integer workspace memory <option-IPOPT-ma27_integer_workspace_memory>` 
     - ma27_liw_init_factor
   * - :ref:`Linear solver - MA27 maximum pivot tolerance <option-IPOPT-ma27_maximum_pivot_tolerance>` 
     - ma27_pivtolmax
   * - :ref:`Linear solver - MA27 pivot tolerance <option-IPOPT-ma27_pivot_tolerance>` 
     - ma27_pivtol
   * - :ref:`Linear solver - MA27 real workspace memory <option-IPOPT-ma27_real_workspace_memory>` 
     - ma27_la_init_factor
   * - :ref:`Linear solver - MA57 block size <option-IPOPT-ma57_block_size>` 
     - ma57_block_size
   * - :ref:`Linear solver - MA57 maximum pivot tolerance <option-IPOPT-ma57_maximum_pivot_tolerance>` 
     - ma57_pivtolmax
   * - :ref:`Linear solver - MA57 node amalgamation parameter <option-IPOPT-ma57_node_amalgamation_parameter>` 
     - ma57_node_amalgamation
   * - :ref:`Linear solver - MA57 pivot order <option-IPOPT-ma57_pivot_order>` 
     - ma57_pivot_order
   * - :ref:`Linear solver - MA57 pivot tolerance <option-IPOPT-ma57_pivot_tolerance>` 
     - ma57_pivtol
   * - :ref:`Linear solver - MA57 scaling <option-IPOPT-ma57_scaling>` 
     - ma57_automatic_scaling
   * - :ref:`Linear solver - MA57 small pivot parameter <option-IPOPT-ma57_small_pivot_parameter>` 
     - ma57_small_pivot_flag
   * - :ref:`Linear solver - MA57 work space memory safety factor <option-IPOPT-ma57_work_space_memory_safety_factor>` 
     - ma57_pre_alloc
   * - :ref:`Linear solver - MA77 maximum pivot tolerance <option-IPOPT-ma77_maximum_pivot_tolerance>` 
     - ma77_umax
   * - :ref:`Linear solver - MA77 pivot tolerance <option-IPOPT-ma77_pivot_tolerance>` 
     - ma77_u
   * - :ref:`Linear solver - MA86 maximum pivot tolerance <option-IPOPT-ma86_maximum_pivot_tolerance>` 
     - ma86_umax
   * - :ref:`Linear solver - MA86 pivot tolerance <option-IPOPT-ma86_pivot_tolerance>` 
     - ma86_u
   * - :ref:`Linear solver - MA97 maximum pivot tolerance <option-IPOPT-ma97_maximum_pivot_tolerance>` 
     - ma97_umax
   * - :ref:`Linear solver - MA97 pivot tolerance <option-IPOPT-ma97_pivot_tolerance>` 
     - ma97_u
   * - :ref:`Linear solver - Maximum number of refinement steps <option-IPOPT-maximum_number_of_refinement_steps>` 
     - max_refinement_steps
   * - :ref:`Linear solver - Minimum number of refinement steps <option-IPOPT-minimum_number_of_refinement_steps>` 
     - min_refinement_steps
   * - :ref:`Linear solver - MUMPS maximum pivot tolerance <option-IPOPT-mumps_maximum_pivot_tolerance>` 
     - mumps_pivtolmax
   * - :ref:`Linear solver - MUMPS permuting and scaling <option-IPOPT-mumps_permuting_and_scaling>` 
     - mumps_permuting_scaling
   * - :ref:`Linear solver - MUMPS pivot order <option-IPOPT-mumps_pivot_order>` 
     - mumps_pivot_order
   * - :ref:`Linear solver - MUMPS pivot tolerance <option-IPOPT-mumps_pivot_tolerance>` 
     - mumps_pivtol
   * - :ref:`Linear solver - MUMPS scaling <option-IPOPT-mumps_scaling>` 
     - mumps_scaling
   * - :ref:`Linear solver - MUMPS working space percentage increase <option-IPOPT-mumps_working_space_percentage_increase>` 
     - mumps_mem_percent
   * - :ref:`Multipliers - Constraint multipliers step size method <option-IPOPT-constraint_multipliers_step_size_method>` 
     - alpha_for_y
   * - :ref:`Multipliers - Equality multipliers switch tolerance <option-IPOPT-equality_multipliers_switch_tolerance>` 
     - alpha_for_y_tol
   * - :ref:`Multipliers - Recalculate constraint multipliers <option-IPOPT-recalculate_constraint_multipliers>` 
     - recalc_y
   * - :ref:`Multipliers - Recalculate constraint multipliers tolerance <option-IPOPT-recalculate_constraint_multipliers_tolerance>` 
     - recalc_y_feas_tol
   * - :ref:`NLP - Assume equality constraints are linear <option-IPOPT-assume_equality_constraints_are_linear>` 
     - jac_c_constant
   * - :ref:`NLP - Assume inequality constraints are linear <option-IPOPT-assume_inequality_constraints_are_linear>` 
     - jac_d_constant
   * - :ref:`NLP - Assume quadratic problem <option-IPOPT-assume_quadratic_problem>` 
     - hessian_constant
   * - :ref:`NLP - Check derivatives for invalid numbers <option-IPOPT-check_derivatives_for_invalid_numbers>` 
     - check_derivatives_for_naninf
   * - :ref:`NLP - Factor for initial bounds relaxation <option-IPOPT-factor_for_initial_bounds_relaxation>` 
     - bound_relax_factor
   * - :ref:`NLP - Fixed variable handling <option-IPOPT-fixed_variable_handling>` 
     - fixed_variable_treatment
   * - :ref:`NLP - Honor original bounds <option-IPOPT-honor_original_bounds>` 
     - honor_original_bounds
   * - :ref:`NLP - Infinity upper bound <option-IPOPT-infinity_upper_bound>` 
     - nlp_upper_bound_inf
   * - :ref:`NLP - Minus infinity lower bound <option-IPOPT-minus_infinity_lower_bound>` 
     - nlp_lower_bound_inf
   * - :ref:`NLP scaling - Maximum gradient after NLP scaling <option-IPOPT-maximum_gradient_after_nlp_scaling>` 
     - nlp_scaling_max_gradient
   * - :ref:`NLP scaling - NLP scaling method <option-IPOPT-nlp_scaling_method>` 
     - nlp_scaling_method
   * - :ref:`NLP scaling - Objective function scaling factor <option-IPOPT-objective_function_scaling_factor>` 
     - obj_scaling_factor
   * - :ref:`Output - Output verbosity level <option-IPOPT-output_verbosity_level>` 
     - print_level
   * - :ref:`Output - Print all available algorithmic options <option-IPOPT-print_all_available_algorithmic_options>` 
     - print_options_documentation
   * - :ref:`Output - Print all user selected options <option-IPOPT-print_all_user_selected_options>` 
     - print_user_options
   * - :ref:`Output - Status file <option-IPOPT-status_file>` 
     - 
   * - :ref:`Quasi-Newton - Hessian approximation history memory limit <option-IPOPT-hessian_approximation_history_memory_limit>` 
     - limited_memory_max_history
   * - :ref:`Quasi-Newton - Hessian approximation successive iterations limit <option-IPOPT-hessian_approximation_successive_iterations_limit>` 
     - limited_memory_max_skipping
   * - :ref:`Quasi-Newton - Method for Hessian computation <option-IPOPT-method_for_hessian_computation>` 
     - hessian_approximation
   * - :ref:`Restoration phase - Bound multipliers reset threshold <option-IPOPT-bound_multipliers_reset_threshold>` 
     - bound_mult_reset_threshold
   * - :ref:`Restoration phase - Constraint multipliers reset threshold <option-IPOPT-constraint_multipliers_reset_threshold>` 
     - constr_mult_reset_threshold
   * - :ref:`Restoration phase - Force start in restoration phase <option-IPOPT-force_start_in_restoration_phase>` 
     - start_with_resto
   * - :ref:`Restoration phase - Maximum multipliers infeasible problem <option-IPOPT-maximum_multipliers_infeasible_problem>` 
     - expect_infeasible_problem_ytol
   * - :ref:`Restoration phase - Minimum violation infeasible problem <option-IPOPT-minimum_violation_infeasible_problem>` 
     - expect_infeasible_problem_ctol
   * - :ref:`Restoration phase - Quickly detect infeasible problem <option-IPOPT-quickly_detect_infeasible_problem>` 
     - expect_infeasible_problem
   * - :ref:`Restoration phase - Reduction factor primal dual error <option-IPOPT-reduction_factor_primal_dual_error>` 
     - soft_resto_pderror_reduction_factor
   * - :ref:`Restoration phase - Required infeasibility reduction <option-IPOPT-required_infeasibility_reduction>` 
     - required_infeasibility_reduction
   * - :ref:`Restoration phase - Use original objective function in restoration phase <option-IPOPT-use_original_objective_function_in_restoration_phase>` 
     - evaluate_orig_obj_at_resto_trial
   * - :ref:`Termination - Acceptable complementarity tolerance <option-IPOPT-acceptable_complementarity_tolerance>` 
     - acceptable_compl_inf_tol
   * - :ref:`Termination - Acceptable constraint violation tolerance <option-IPOPT-acceptable_constraint_violation_tolerance>` 
     - acceptable_constr_viol_tol
   * - :ref:`Termination - Acceptable dual infeasibility tolerance <option-IPOPT-acceptable_dual_infeasibility_tolerance>` 
     - acceptable_dual_inf_tol
   * - :ref:`Termination - Acceptable objective change tolerance <option-IPOPT-acceptable_objective_change_tolerance>` 
     - acceptable_obj_change_tol
   * - :ref:`Termination - Acceptable relative convergence tolerance <option-IPOPT-acceptable_relative_convergence_tolerance>` 
     - acceptable_tol
   * - :ref:`Termination - Complementarity tolerance <option-IPOPT-complementarity_tolerance>` 
     - compl_inf_tol
   * - :ref:`Termination - Constraint violation tolerance <option-IPOPT-constraint_violation_tolerance>` 
     - constr_viol_tol
   * - :ref:`Termination - Diverging iterates tolerance <option-IPOPT-diverging_iterates_tolerance>` 
     - diverging_iterates_tol
   * - :ref:`Termination - Dual infeasibility tolerance <option-IPOPT-dual_infeasibility_tolerance>` 
     - dual_inf_tol
   * - :ref:`Termination - Maximum number of acceptable iterations <option-IPOPT-maximum_number_of_acceptable_iterations>` 
     - acceptable_iter
   * - :ref:`Termination - Maximum number of iterations <option-IPOPT-maximum_number_of_iterations>` 
     - max_iter
   * - :ref:`Termination - Relative convergence tolerance <option-IPOPT-relative_convergence_tolerance>` 
     - tol
