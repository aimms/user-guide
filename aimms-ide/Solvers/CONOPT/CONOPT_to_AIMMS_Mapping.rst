.. _CONOPT_to_AIMMS_Mapping:


CONOPT to AIMMS Mapping
=======================

**Description** 

The table shows in the left column the parameters from CONOPT that can be set in AIMMS; the right column displays for each CONOPT parameter the associated AIMMS option.
	
.. list-table::

   * - **Name in CONOPT**
     - **Option name in AIMMS**
   * - DOINTV
     - :ref:`Preprocessing - Use Interval Evaluations <option-CONOPT-use_interval_evaluations>`
   * - DONOPEN
     - :ref:`Advanced - Use No-Penalty Model <option-CONOPT-use_no-penalty_model>`
   * - DOPREP
     - :ref:`Preprocessing - Preprocessor <option-CONOPT-preprocessor>`
   * - LF2DRV
     - :ref:`Limits - Limit on Directional 2nd Order Derivative Errors <option-CONOPT-limit_on_directional_2nd_order_derivative_errors>`
   * - LFDEGI
     - :ref:`Limits - Limit on Degenerate Iterations <option-CONOPT-limit_on_degenerate_iterations>`
   * - LFHSOK
     - :ref:`Limits - Limit on Hessian Evaluation Errors <option-CONOPT-limit_on_hessian_evaluation_errors>`
   * - LFILOG
     - :ref:`Reporting - Log Frequency <option-CONOPT-log_frequency>`
   * - LFILOS
     - :ref:`Reporting - Log Frequency SLP and SQP <option-CONOPT-log_frequency_slp_and_sqp>`
   * - LFITER
     - :ref:`Stop Criteria - Iteration Limit <option-AIMMS-iteration_limit>`  in 'Solvers - General'
   * - LFMXNS
     - :ref:`Limits - Limit on New Superbasics <option-CONOPT-limit_on_new_superbasics>`
   * - LFNICR
     - :ref:`Stop criteria - Limit for Slow Progress <option-CONOPT-limit_for_slow_progress>`
   * - LFNSUP
     - :ref:`Limits - Maximal Hessian Dimension <option-CONOPT-maximal_hessian_dimension>`
   * - LFSCAL
     - :ref:`Scaling - Rescale Frequency <option-CONOPT-rescale_frequency>`
   * - LFSTAL
     - :ref:`Stop criteria - Maximal Number of Stalled Iterations <option-CONOPT-maximal_number_of_stalled_iterations>`
   * - LFUSDF
     - :ref:`Limits - Limit on Candidates for Defined Variable <option-CONOPT-limit_on_candidates_for_defined_variable>`
   * - LKDEB2
     - :ref:`Debugging - Check 2nd Order Derivatives <option-CONOPT-check_2nd_order_derivatives>`
   * - LKDEBG
     - :ref:`Debugging - Check 1st Order Derivatives <option-CONOPT-check_1st_order_derivatives>`
   * - LMETHOD
     - :ref:`Advanced - Method for Linear Feasibility Models <option-CONOPT-method_for_linear_feasibility_models>`
   * - LMMXSF
     - :ref:`Advanced - Method for Finding Maximal Step <option-CONOPT-method_for_finding_maximal_step>`
   * - LMMXST
     - :ref:`Advanced - Method for Finding Maximal Tight Step <option-CONOPT-method_for_finding_maximal_tight_step>`
   * - LMNDIA
     - :ref:`Advanced - Method for Reduced Hessian <option-CONOPT-method_for_reduced_hessian>`
   * - LMSCAL
     - :ref:`Scaling - Scaling Method <option-CONOPT-scaling_method>`
   * - LMUSDF
     - :ref:`Advanced - Method for Defined Variables <option-CONOPT-method_for_defined_variables>`
   * - LSCRSH
     - :ref:`General - Method for Initial Basis <option-CONOPT-method_for_initial_basis>`
   * - LSESLP
     - :ref:`Advanced - SLP Mode <option-CONOPT-slp_mode>`
   * - LSESQP
     - :ref:`Advanced - SQP Mode <option-CONOPT-sqp_mode>`
   * - LSLACK
     - :ref:`Advanced - Logical Switch for Selection of Slacks <option-CONOPT-logical_switch_for_selection_of_slacks>`
   * - LSSQRS
     - :ref:`General - Model is Square System <option-CONOPT-model_is_square_system>`
   * - ISCONVEX
     - :ref:`General - Model is Convex <option-CONOPT-model_is_convex>`
   * - NROUNDS
     - :ref:`Limits - Limit on Linear Feasibility Model Rounds <option-CONOPT-limit_on_linear_feasibility_model_rounds>`
   * - RT2DRV
     - :ref:`Debugging - Tolerance 2nd Order Derivatives Check <option-CONOPT-tolerance_2nd_order_derivatives_check>`
   * - RTBND1
     - :ref:`General - Bound Tolerance <option-CONOPT-bound_tolerance>`
   * - RTBNDI
     - :ref:`Advanced - Fixed Variables Tolerance Initial Bounds <option-CONOPT-fixed_variables_tolerance_initial_bounds>`
   * - RTBNDT
     - :ref:`Advanced - Fixed Variables Tolerance Derived Bounds <option-CONOPT-fixed_variables_tolerance_derived_bounds>`
   * - RTBOX
     - :ref:`Advanced - Box Size Tolerance <option-CONOPT-box_size_tolerance>`
   * - RTBOXF
     - :ref:`Advanced - Box Size Factor Linear Variables <option-CONOPT-box_size_factor_linear_variables>`
   * - RTBOXL
     - :ref:`Advanced - Box Size Tolerance Linear <option-CONOPT-box_size_tolerance_linear>`
   * - RTIPVA
     - :ref:`Pivot - Absolute Pivot Tolerance Initial Basis <option-CONOPT-absolute_pivot_tolerance_initial_basis>`
   * - RTIPVR
     - :ref:`Pivot - Relative Pivot Tolerance Initial Basis <option-CONOPT-relative_pivot_tolerance_initial_basis>`
   * - RTMAXS
     - :ref:`Scaling - Maximal Scaling Factor <option-CONOPT-maximal_scaling_factor>`
   * - RTMAXV
     - :ref:`Limits - Maximum Solution of a Variable <option-CONOPT-maximum_solution_of_a_variable>`
   * - RTMINA
     - :ref:`Advanced - Zero Filter Tolerance Jacobian Elements <option-CONOPT-zero_filter_tolerance_jacobian_elements>`
   * - RTMINJ
     - :ref:`Scaling - Minimal Jacobian Element for Scaling <option-CONOPT-minimal_jacobian_element_for_scaling>`
   * - RTMINS
     - :ref:`Scaling - Minimal Scaling Factor <option-CONOPT-minimal_scaling_factor>`
   * - RTMINV
     - :ref:`Scaling - Minimal Scaling Tolerance for Variables <option-CONOPT-minimal_scaling_tolerance_for_variables>`
   * - RTMNS2
     - :ref:`Scaling - Minimal Scaling Factor 2nd Order Derivatives <option-CONOPT-minimal_scaling_factor_2nd_order_derivatives>`
   * - RTNOPN
     - :ref:`Advanced - Penalty Constraints Ratio <option-CONOPT-penalty_constraints_ratio>`
   * - RTNWMA
     - :ref:`General - Maximal Feasibility Tolerance <option-CONOPT-maximal_feasibility_tolerance>`
   * - RTNWMI
     - :ref:`General - Minimal Feasibility Tolerance <option-CONOPT-minimal_feasibility_tolerance>`
   * - RTNWTR
     - :ref:`General - Feasibility Tolerance Triangular Part <option-CONOPT-feasibility_tolerance_triangular_part>`
   * - RTOBJL
     - :ref:`Stop criteria - Slow Progress Tolerance <option-CONOPT-slow_progress_tolerance>`
   * - RTOBJR
     - :ref:`Advanced - Relative Objective Accuracy <option-CONOPT-relative_objective_accuracy>`
   * - RTONED
     - :ref:`Stop criteria - Accuracy One Dimensional Search <option-CONOPT-accuracy_one_dimensional_search>`
   * - RTPIVA
     - :ref:`Pivot - Absolute Pivot Tolerance <option-CONOPT-absolute_pivot_tolerance>`
   * - RTPIVR
     - :ref:`Pivot - Relative Pivot Tolerance <option-CONOPT-relative_pivot_tolerance>`
   * - RTPIVS
     - :ref:`Pivot - Relative Pivot Tolerance during Ratio Test <option-CONOPT-relative_pivot_tolerance_during_ratio_test>`
   * - RTPIVT
     - :ref:`Pivot - Absolute Pivot Tolerance Nonlinear Elements <option-CONOPT-absolute_pivot_tolerance_nonlinear_elements>`
   * - RTPIVU
     - :ref:`Pivot - Relative Pivot Tolerance during Basis Updates <option-CONOPT-relative_pivot_tolerance_during_basis_updates>`
   * - RTREDG
     - :ref:`Stop criteria - Optimality Tolerance <option-CONOPT-optimality_tolerance>`
   * - RTREDI
     - :ref:`Stop criteria - Optimality Tolerance Infeasible <option-CONOPT-optimality_tolerance_infeasible>`
   * - RVSTLM
     - :ref:`Advanced - Steplength Multiplier <option-CONOPT-steplength_multiplier>`
   * - RVTIME
     - :ref:`Stop Criteria - Time Limit <option-AIMMS-time_limit>`  in 'Solvers - General'
