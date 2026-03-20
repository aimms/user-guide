

.. _AIMMS_to_IPOPT_Mapping:


AIMMS to IPOPT Mapping
======================

**Description** 

The table shows in the left column the AIMMS IPOPT options while the right column displays the associated IPOPT parameter.

.. list-table::

   * - **Option name in AIMMS** 
     - **Name in IPOPT** 
   * - :doc:`Barrier parameter - Adaptive strategy factor limit <Barrier parameter/IPOPT_Barrier_-_Adaptive_strategy_factor_limit>` 
     - mu_max_fact
   * - :doc:`Barrier parameter - Adaptive strategy oracle <Barrier parameter/IPOPT_Barrier_-_Adaptive_strategy_oracle>` 
     - mu_oracle
   * - :doc:`Barrier parameter - Barrier convergence tolerance factor <Barrier parameter/IPOPT_Barrier_-_Barrier_convergence_tolerance_factor>` 
     - barrier_tol_factor
   * - :doc:`Barrier parameter - Barrier parameter initial value <Barrier parameter/IPOPT_Barrier_-_Barrier_parameter_initial_value>` 
     - mu_init
   * - :doc:`Barrier parameter - Barrier parameter update strategy <Barrier parameter/IPOPT_Barrier_-_Barrier_parameter_update_strategy>` 
     - mu_strategy
   * - :doc:`Barrier parameter - Execute Mehrotra algorithm <Barrier parameter/IPOPT_Barrier_-_Execute_Mehrotra_algorithm>` 
     - mehrotra_algorithm
   * - :doc:`Barrier parameter - Fixed mode oracle <Barrier parameter/IPOPT_Barrier_-_Fixed_mode_oracle>` 
     - fixed_mu_oracle
   * - :doc:`Barrier parameter - Linear decrease factor barrier parameter <Barrier parameter/IPOPT_Barrier_-_Linear_decrease_factor_barrier_parameter>` 
     - mu_linear_decrease_factor
   * - :doc:`Barrier parameter - Maximum value for barrier parameter <Barrier parameter/IPOPT_Barrier_-_Maximum_value_for_barrier_parameter>` 
     - mu_max
   * - :doc:`Barrier parameter - Minimum value for barrier parameter <Barrier parameter/IPOPT_Barrier_-_Minimum_value_for_barrier_parameter>` 
     - mu_min
   * - :doc:`Barrier parameter - Quality function section steps limit <Barrier parameter/IPOPT_Barrier_-_Quality_function_section_steps_limit>` 
     - quality_function_max_section_steps
   * - :doc:`Barrier parameter - Superlinear decrease rate barrier parameter <Barrier parameter/IPOPT_Barrier_-_Superlinear_decrease_rate_barrier_parameter>` 
     - mu_superlinear_decrease_power
   * - :doc:`Derivative test - Derivative checker verbosity <Derivative test/IPOPT_Derivative_test_-_Derivative_checker_verbosity>` 
     - derivative_test_print_all
   * - :doc:`Derivative test - Derivative test perturbation size <Derivative test/IPOPT_Derivative_test_-_Derivative_test_perturbation_size>` 
     - derivative_test_perturbation
   * - :doc:`Derivative test - Derivative test tolerance <Derivative test/IPOPT_Derivative_test_-_Derivative_test_tolerance>` 
     - derivative_test_tol
   * - :doc:`Derivative test - Derivative testing <Derivative test/IPOPT_Derivative_test_-_Derivative_testing>` 
     - derivative_test
   * - :doc:`Derivative test - Maximum perturbation of evaluation point <Derivative test/IPOPT_Derivative_test_-_Maximum_perturbation_of_evaluation_point>` 
     - point_perturbation_radius
   * - :doc:`Hessian perturbation - First Hessian perturbation increase factor <Hessian perturbation/IPOPT_Hessian_perturbation_-_First_Hessian_perturbation_increase_factor>` 
     - perturb_inc_fact_first
   * - :doc:`Hessian perturbation - First Hessian perturbation size <Hessian perturbation/IPOPT_Hessian_perturbation_-_First_Hessian_perturbation_size>` 
     - first_hessian_perturbation
   * - :doc:`Hessian perturbation - Hessian perturbation decrease factor <Hessian perturbation/IPOPT_Hessian_perturbation_-_Hessian_perturbation_decrease_factor>` 
     - perturb_dec_fact
   * - :doc:`Hessian perturbation - Hessian perturbation increase factor <Hessian perturbation/IPOPT_Hessian_perturbation_-_Hessian_perturbation_increase_factor>` 
     - perturb_inc_fact
   * - :doc:`Hessian perturbation - Jacobian regularization value <Hessian perturbation/IPOPT_Hessian_perturbation_-_Jacobian_regularization_value>` 
     - jacobian_regularization_value
   * - :doc:`Hessian perturbation - Maximum Hessian perturbation <Hessian perturbation/IPOPT_Hessian_perturbation_-_Maximum_Hessian_perturbation>` 
     - max_hessian_perturbation
   * - :doc:`Hessian perturbation - Minimum Hessian perturbation <Hessian perturbation/IPOPT_Hessian_perturbation_-_Minimum_Hessian_perturbation>` 
     - min_hessian_perturbation
   * - :doc:`Initialization - Bound multipliers initialization method <Initialization/IPOPT_Initialization_-_Bound_multipliers_initialization_method>` 
     - bound_mult_init_method
   * - :doc:`Initialization - Constraint multipliers initial guess limit <Initialization/IPOPT_Initialization_-_Constraint_multipliers_initial_guess_limit>` 
     - constr_mult_init_max
   * - :doc:`Initialization - Initial value for bound multipliers <Initialization/IPOPT_Initialization_-_Initial_value_for_bound_multipliers>` 
     - bound_mult_init_val
   * - :doc:`Initialization - Point to bound absolute distance <Initialization/IPOPT_Initialization_-_Point_to_bound_absolute_distance>` 
     - bound_push
   * - :doc:`Initialization - Point to bound relative distance <Initialization/IPOPT_Initialization_-_Point_to_bound_relative_distance>` 
     - bound_frac
   * - :doc:`Initialization - Slack to bound absolute distance <Initialization/IPOPT_Initialization_-_Slack_to_bound_absolute_distance>` 
     - slack_bound_push
   * - :doc:`Initialization - Slack to bound relative distance <Initialization/IPOPT_Initialization_-_Slack_to_bound_relative_distance>` 
     - slack_bound_frac
   * - :doc:`Line search - Always accept full trial step <Line search/IPOPT_Line_search_-_Always_accept_full_trial_step>` 
     - accept_every_trial_step
   * - :doc:`Line search - Corrector steps type <Line search/IPOPT_Line_search_-_Corrector_steps_type>` 
     - corrector_type
   * - :doc:`Line search - Maximum number of watchdog iterations <Line search/IPOPT_Line_search_-_Maximum_number_of_watchdog_iterations>` 
     - watchdog_trial_iter_max
   * - :doc:`Line search - Second order correction trial steps limit <Line search/IPOPT_Line_search_-_Second_order_correction_trial_steps_limit>` 
     - max_soc
   * - :doc:`Line search - Watchdog shortened iteration trigger <Line search/IPOPT_Line_search_-_Watchdog_shortened_iteration_trigger>` 
     - watchdog_shortened_iter_trigger
   * - :doc:`Linear solver - Linear solver selection <Linear solver/IPOPT_Linear_solver_-_Linear_solver_selection>` 
     - linear_solver
   * - :doc:`Linear solver - Linear system scaling <Linear solver/IPOPT_Linear_solver_-_Linear_system_scaling>` 
     - linear_scaling_on_demand
   * - :doc:`Linear solver - Linear system scaling method <Linear solver/IPOPT_Linear_solver_-_Linear_system_scaling_method>` 
     - linear_system_scaling
   * - :doc:`Linear solver - MA27 increment factor for workspace size <Linear solver/IPOPT_Linear_solver_-_MA27_increment_factor_for_workspace_size>` 
     - ma27_meminc_factor
   * - :doc:`Linear solver - MA27 integer workspace memory <Linear solver/IPOPT_Linear_solver_-_MA27_integer_workspace_memory>` 
     - ma27_liw_init_factor
   * - :doc:`Linear solver - MA27 maximum pivot tolerance <Linear solver/IPOPT_Linear_solver_-_MA27_maximum_pivot_tolerance>` 
     - ma27_pivtolmax
   * - :doc:`Linear solver - MA27 pivot tolerance <Linear solver/IPOPT_Linear_solver_-_MA27_pivot_tolerance>` 
     - ma27_pivtol
   * - :doc:`Linear solver - MA27 real workspace memory <Linear solver/IPOPT_Linear_solver_-_MA27_real_workspace_memory>` 
     - ma27_la_init_factor
   * - :doc:`Linear solver - MA57 block size <Linear solver/IPOPT_Linear_solver_-_MA57_block_size>` 
     - ma57_block_size
   * - :doc:`Linear solver - MA57 maximum pivot tolerance <Linear solver/IPOPT_Linear_solver_-_MA57_maximum_pivot_tolerance>` 
     - ma57_pivtolmax
   * - :doc:`Linear solver - MA57 node amalgamation parameter <Linear solver/IPOPT_Linear_solver_-_MA57_node_amalgamation_paramet>` 
     - ma57_node_amalgamation
   * - :doc:`Linear solver - MA57 pivot order <Linear solver/IPOPT_Linear_solver_-_MA57_pivot_order>` 
     - ma57_pivot_order
   * - :doc:`Linear solver - MA57 pivot tolerance <Linear solver/IPOPT_Linear_solver_-_MA57_pivot_tolerance>` 
     - ma57_pivtol
   * - :doc:`Linear solver - MA57 scaling <Linear solver/IPOPT_Linear_solver_-_MA57_scaling>` 
     - ma57_automatic_scaling
   * - :doc:`Linear solver - MA57 small pivot parameter <Linear solver/IPOPT_Linear_solver_-_MA57_small_pivot_parameter>` 
     - ma57_small_pivot_flag
   * - :doc:`Linear solver - MA57 work space memory safety factor <Linear solver/IPOPT_Linear_solver_-_MA57_work_space_memory_safety_f>` 
     - ma57_pre_alloc
   * - :doc:`Linear solver - MA77 maximum pivot tolerance <Linear solver/IPOPT_Linear_solver_-_MA77_maximum_pivot_tolerance>` 
     - ma77_umax
   * - :doc:`Linear solver - MA77 pivot tolerance <Linear solver/IPOPT_Linear_solver_-_MA77_pivot_tolerance>` 
     - ma77_u
   * - :doc:`Linear solver - MA86 maximum pivot tolerance <Linear solver/IPOPT_Linear_solver_-_MA86_maximum_pivot_tolerance>` 
     - ma86_umax
   * - :doc:`Linear solver - MA86 pivot tolerance <Linear solver/IPOPT_Linear_solver_-_MA86_pivot_tolerance>` 
     - ma86_u
   * - :doc:`Linear solver - MA97 maximum pivot tolerance <Linear solver/IPOPT_Linear_solver_-_MA97_maximum_pivot_tolerance>` 
     - ma97_umax
   * - :doc:`Linear solver - MA97 pivot tolerance <Linear solver/IPOPT_Linear_solver_-_MA97_pivot_tolerance>` 
     - ma97_u
   * - :doc:`Linear solver - Maximum number of refinement steps <Linear solver/IPOPT_Linear_solver_-_Maximum_number_of_refinement_steps>` 
     - max_refinement_steps
   * - :doc:`Linear solver - Minimum number of refinement steps <Linear solver/IPOPT_Linear_solver_-_Minimum_number_of_refinement_steps>` 
     - min_refinement_steps
   * - :doc:`Linear solver - MUMPS maximum pivot tolerance <Linear solver/IPOPT_Linear_solver_-_MUMPS_maximum_pivot_tolerance>` 
     - mumps_pivtolmax
   * - :doc:`Linear solver - MUMPS permuting and scaling <Linear solver/IPOPT_Linear_solver_-_MUMPS_permuting_and_scaling>` 
     - mumps_permuting_scaling
   * - :doc:`Linear solver - MUMPS pivot order <Linear solver/IPOPT_Linear_solver_-_MUMPS_pivot_order>` 
     - mumps_pivot_order
   * - :doc:`Linear solver - MUMPS pivot tolerance <Linear solver/IPOPT_Linear_solver_-_MUMPS_pivot_tolerance>` 
     - mumps_pivtol
   * - :doc:`Linear solver - MUMPS scaling <Linear solver/IPOPT_Linear_solver_-_MUMPS_scaling>` 
     - mumps_scaling
   * - :doc:`Linear solver - MUMPS working space percentage increase <Linear solver/IPOPT_Linear_solver_-_MUMPS_working_space_percentage_increase>` 
     - mumps_mem_percent
   * - :doc:`Multipliers - Constraint multipliers step size method <Multipliers/IPOPT_Multipliers_-_Constraint_multipliers_step_size_method>` 
     - alpha_for_y
   * - :doc:`Multipliers - Equality multipliers switch tolerance <Multipliers/IPOPT_Multipliers_-_Equality_multipliers_switch_tolerance>` 
     - alpha_for_y_tol
   * - :doc:`Multipliers - Recalculate constraint multipliers <Multipliers/IPOPT_Multipliers_-_Recalculate_constraint_multipliers>` 
     - recalc_y
   * - :doc:`Multipliers - Recalculate constraint multipliers tolerance <Multipliers/IPOPT_Multipliers_-_Recalculate_constraint_multipliers_tolerance>` 
     - recalc_y_feas_tol
   * - :doc:`NLP - Assume equality constraints are linear <NLP/IPOPT_NLP_-_Assume_equality_constraints_are_linear>` 
     - jac_c_constant
   * - :doc:`NLP - Assume inequality constraints are linear <NLP/IPOPT_NLP_-_Assume_inequality_constraints_are_linear>` 
     - jac_d_constant
   * - :doc:`NLP - Assume quadratic problem <NLP/IPOPT_NLP_-_Assume_quadratic_problem>` 
     - hessian_constant
   * - :doc:`NLP - Check derivatives for invalid numbers <NLP/IPOPT_NLP_-_Check_derivatives_for_invalid_numbers>` 
     - check_derivatives_for_naninf
   * - :doc:`NLP - Factor for initial bounds relaxation <NLP/IPOPT_NLP_-_Factor_for_initial_bounds_relaxation>` 
     - bound_relax_factor
   * - :doc:`NLP - Fixed variable handling <NLP/IPOPT_NLP_-_Fixed_variable_handling>` 
     - fixed_variable_treatment
   * - :doc:`NLP - Honor original bounds <NLP/IPOPT_NLP_-_Honor_original_bounds>` 
     - honor_original_bounds
   * - :doc:`NLP - Infinity upper bound <NLP/IPOPT_NLP_-_Infinity_upper_bound>` 
     - nlp_upper_bound_inf
   * - :doc:`NLP - Minus infinity lower bound <NLP/IPOPT_NLP_-_Minus_infinity_lower_bound>` 
     - nlp_lower_bound_inf
   * - :doc:`NLP scaling - Maximum gradient after NLP scaling <NLP scaling/IPOPT_NLP_scaling_-_Maximum_gradient_after_NLP_scaling>` 
     - nlp_scaling_max_gradient
   * - :doc:`NLP scaling - NLP scaling method <NLP scaling/IPOPT_NLP_scaling_-_NLP_scaling_method>` 
     - nlp_scaling_method
   * - :doc:`NLP scaling - Objective function scaling factor <NLP scaling/IPOPT_NLP_scaling_-_Objective_function_scaling_factor>` 
     - obj_scaling_factor
   * - :doc:`Output - Output verbosity level <Output/IPOPT_Output_-_Output_verbosity_level>` 
     - print_level
   * - :doc:`Output - Print all available algorithmic options <Output/IPOPT_Output_-_Print_all_available_algorithmic_options>` 
     - print_options_documentation
   * - :doc:`Output - Print all user selected options <Output/IPOPT_Output_-_Print_all_user_selected_options>` 
     - print_user_options
   * - :doc:`Output - Status file <Output/IPOPT_Output_-_Status_file>` 
     - 
   * - :doc:`Quasi-Newton - Hessian approximation history memory limit <Quasi-Newton/IPOPT_Quasi-Newton_-_Hessian_approximation_history_memory_limit>` 
     - limited_memory_max_history
   * - :doc:`Quasi-Newton - Hessian approximation successive iterations limit <Quasi-Newton/IPOPT_Quasi-Newton_-_Hessian_approximation_successive_iterations_limit>` 
     - limited_memory_max_skipping
   * - :doc:`Quasi-Newton - Method for Hessian computation <Quasi-Newton/IPOPT_Quasi-Newton_-_Method_for_Hessian_computation>` 
     - hessian_approximation
   * - :doc:`Restoration phase - Bound multipliers reset threshold <Restoration phase/IPOPT_Restoration_phase_-_Bound_multipliers_reset_threshold>` 
     - bound_mult_reset_threshold
   * - :doc:`Restoration phase - Constraint multipliers reset threshold <Restoration phase/IPOPT_Restoration_phase_-_Constraint_multipliers_reset_threshold>` 
     - constr_mult_reset_threshold
   * - :doc:`Restoration phase - Force start in restoration phase <Restoration phase/IPOPT_Restoration_phase_-_Force_start_in_restoration_phase>` 
     - start_with_resto
   * - :doc:`Restoration phase - Maximum multipliers infeasible problem <Restoration phase/IPOPT_Restoration_phase_-_Maximum_multipliers_infeasible_problem>` 
     - expect_infeasible_problem_ytol
   * - :doc:`Restoration phase - Minimum violation infeasible problem <Restoration phase/IPOPT_Restoration_phase_-_Minimum_violation_infeasible_problem>` 
     - expect_infeasible_problem_ctol
   * - :doc:`Restoration phase - Quickly detect infeasible problem <Restoration phase/IPOPT_Restoration_phase_-_Quickly_detect_infeasible_problem>` 
     - expect_infeasible_problem
   * - :doc:`Restoration phase - Reduction factor primal dual error <Restoration phase/IPOPT_Restoration_phase_-_Reduction_factor_primal_dual_error>` 
     - soft_resto_pderror_reduction_factor
   * - :doc:`Restoration phase - Required infeasibility reduction <Restoration phase/IPOPT_Restoration_phase_-_Required_infeasibility_reduction>` 
     - required_infeasibility_reduction
   * - :doc:`Restoration phase - Use original objective function in restoration phase <Restoration phase/IPOPT_Restoration_phase_-_Use_original_objective_function_in_restoration_phase>` 
     - evaluate_orig_obj_at_resto_trial
   * - :doc:`Termination - Acceptable complementarity tolerance <Termination/IPOPT_Termination_-_Acceptable_complementarity_tolerance>` 
     - acceptable_compl_inf_tol
   * - :doc:`Termination - Acceptable constraint violation tolerance <Termination/IPOPT_Termination_-_Acceptable_constraint_violation_tolerance>` 
     - acceptable_constr_viol_tol
   * - :doc:`Termination - Acceptable dual infeasibility tolerance <Termination/IPOPT_Termination_-_Acceptable_dual_infeasibility_tolerance>` 
     - acceptable_dual_inf_tol
   * - :doc:`Termination - Acceptable objective change tolerance <Termination/IPOPT_Termination_-_Acceptable_objective_change_tolerance>` 
     - acceptable_obj_change_tol
   * - :doc:`Termination - Acceptable relative convergence tolerance <Termination/IPOPT_Termination_-_Acceptable_relative_convergence_tolerance>` 
     - acceptable_tol
   * - :doc:`Termination - Complementarity tolerance <Termination/IPOPT_Termination_-_Complementarity_tolerance>` 
     - compl_inf_tol
   * - :doc:`Termination - Constraint violation tolerance <Termination/IPOPT_Termination_-_Constraint_violation_tolerance>` 
     - constr_viol_tol
   * - :doc:`Termination - Diverging iterates tolerance <Termination/IPOPT_Termination_-_Diverging_iterates_tolerance>` 
     - diverging_iterates_tol
   * - :doc:`Termination - Dual infeasibility tolerance <Termination/IPOPT_Termination_-_Dual_infeasibility_tolerance>` 
     - dual_inf_tol
   * - :doc:`Termination - Maximum number of acceptable iterations <Termination/IPOPT_Termination_-_Maximum_number_of_acceptable_iterations>` 
     - acceptable_iter
   * - :doc:`Termination - Maximum number of iterations <Termination/IPOPT_Termination_-_Maximum_number_of_iterations>` 
     - max_iter
   * - :doc:`Termination - Relative convergence tolerance <Termination/IPOPT_Termination_-_Relative_convergence_tolerance>` 
     - tol
