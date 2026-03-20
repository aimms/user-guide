

.. _AIMMS_to_CONOPT_Mapping:


AIMMS to CONOPT Mapping
=======================

**Description** 

The table shows in the left column the AIMMS CONOPT options; 
the right column displays for the AIMMS option 
the CONOPT parameter that is associated with it.

.. list-table::

   * - **Option name in AIMMS**
     - **Name in CONOPT**
   * - :ref:`Advanced - Box Size Factor Linear Variables <option-CONOPT-box_size_factor_linear_variables>`
     - RTBOXF
   * - :ref:`Advanced - Box Size Tolerance <option-CONOPT-box_size_tolerance>`
     - RTBOX
   * - :ref:`Advanced - Box Size Tolerance Linear <option-CONOPT-box_size_tolerance_linear>`
     - RTBOXL
   * - :ref:`Advanced - Fixed Variables Tolerance Derived Bounds <option-CONOPT-fixed_variables_tolerance_derived_bounds>`
     - RTBNDT
   * - :ref:`Advanced - Fixed Variables Tolerance Initial Bounds <option-CONOPT-fixed_variables_tolerance_initial_bounds>`
     - RTBNDI
   * - :ref:`Advanced - Logical Switch for Selection of Slacks <option-CONOPT-logical_switch_for_selection_of_slacks>`
     - LSLACK
   * - :ref:`Advanced - Method for Defined Variables <option-CONOPT-method_for_defined_variables>`
     - LMUSDF
   * - :ref:`Advanced - Method for Finding Maximal Step <option-CONOPT-method_for_finding_maximal_step>`
     - LMMXSF
   * - :ref:`Advanced - Method for Finding Maximal Tight Step <option-CONOPT-method_for_finding_maximal_tight_step>`
     - LMMXST
   * - :ref:`Advanced - Method for Linear Feasibility Models <option-CONOPT-method_for_linear_feasibility_models>`
     - LMETHOD
   * - :ref:`Advanced - Method for Reduced Hessian <option-CONOPT-method_for_reduced_hessian>`
     - LMNDIA
   * - :ref:`Advanced - Penalty Constraints Ratio <option-CONOPT-penalty_constraints_ratio>`
     - RTNOPN
   * - :ref:`Advanced - Relative Objective Accuracy <option-CONOPT-relative_objective_accuracy>`
     - RTOBJR
   * - :ref:`Advanced - SLP Mode <option-CONOPT-slp_mode>`
     - LSESLP
   * - :ref:`Advanced - SQP Mode <option-CONOPT-sqp_mode>`
     - LSESQP
   * - :ref:`Advanced - Steplength Multiplier <option-CONOPT-steplength_multiplier>`
     - RVSTLM
   * - :ref:`Advanced - Use No-Penalty Model <option-CONOPT-use_no-penalty_model>`
     - DONOPEN
   * - :ref:`Advanced - Zero Filter Tolerance Jacobian Elements <option-CONOPT-zero_filter_tolerance_jacobian_elements>`
     - RTMINA
   * - :ref:`Debugging - Check 1st Order Derivatives <option-CONOPT-check_1st_order_derivatives>`
     - LKDEBG
   * - :ref:`Debugging - Check 2nd Order Derivatives <option-CONOPT-check_2nd_order_derivatives>`
     - LKDEB2
   * - :ref:`Debugging - Tolerance 2nd Order Derivatives Check <option-CONOPT-tolerance_2nd_order_derivatives_check>`
     - RT2DRV
   * - :ref:`General - Bound Tolerance <option-CONOPT-bound_tolerance>`
     - RTBND1
   * - :ref:`General - Feasibility Tolerance Triangular Part <option-CONOPT-feasibility_tolerance_triangular_part>`
     - RTNWTR
   * - :ref:`General - Maximal Feasibility Tolerance <option-CONOPT-maximal_feasibility_tolerance>`
     - RTNWMA
   * - :ref:`General - Method for Initial Basis <option-CONOPT-method_for_initial_basis>`
     - LSCRSH
   * - :ref:`General - Minimal Feasibility Tolerance <option-CONOPT-minimal_feasibility_tolerance>`
     - RTNWMI
   * - :ref:`General - Model is Convex <option-CONOPT-model_is_convex>`
     - ISCONVEX
   * - :ref:`General - Model is Square System <option-CONOPT-model_is_square_system>`
     - LSSQRS
   * - :ref:`Limits - Limit on Candidates for Defined Variable <option-CONOPT-limit_on_candidates_for_defined_variable>`
     - LFUSDF
   * - :ref:`Limits - Limit on Degenerate Iterations <option-CONOPT-limit_on_degenerate_iterations>`
     - LFDEGI
   * - :ref:`Limits - Limit on Directional 2nd Order Derivative Errors <option-CONOPT-limit_on_directional_2nd_order_derivative_errors>`
     - LF2DRV
   * - :ref:`Limits - Limit on Hessian Evaluation Errors <option-CONOPT-limit_on_hessian_evaluation_errors>`
     - LFHSOK
   * - :ref:`Limits - Limit on Linear Feasibility Model Rounds <option-CONOPT-limit_on_linear_feasibility_model_rounds>`
     - NROUNDS
   * - :ref:`Limits - Limit on New Superbasics <option-CONOPT-limit_on_new_superbasics>`
     - LFMXNS
   * - :ref:`Limits - Maximal Hessian Dimension <option-CONOPT-maximal_hessian_dimension>`
     - LFNSUP
   * - :ref:`Limits - Maximum Solution of a Variable <option-CONOPT-maximum_solution_of_a_variable>`
     - RTMAXV
   * - :ref:`Pivot - Absolute Pivot Tolerance <option-CONOPT-absolute_pivot_tolerance>`
     - RTPIVA
   * - :ref:`Pivot - Absolute Pivot Tolerance Initial Basis <option-CONOPT-absolute_pivot_tolerance_initial_basis>`
     - RTIPVA
   * - :ref:`Pivot - Absolute Pivot Tolerance Nonlinear Elements <option-CONOPT-absolute_pivot_tolerance_nonlinear_elements>`
     - RTPIVT
   * - :ref:`Pivot - Relative Pivot Tolerance <option-CONOPT-relative_pivot_tolerance>`
     - RTPIVR
   * - :ref:`Pivot - Relative Pivot Tolerance during Basis Updates <option-CONOPT-relative_pivot_tolerance_during_basis_updates>`
     - RTPIVU
   * - :ref:`Pivot - Relative Pivot Tolerance during Ratio Test <option-CONOPT-relative_pivot_tolerance_during_ratio_test>`
     - RTPIVS
   * - :ref:`Pivot - Relative Pivot Tolerance during Basis Updates <option-CONOPT-relative_pivot_tolerance_during_basis_updates>`
     - RTIPVR
   * - :ref:`Preprocessing - Preprocessor <option-CONOPT-preprocessor>`
     - DOPREP
   * - :ref:`Preprocessing - Use Interval Evaluations <option-CONOPT-use_interval_evaluations>`
     - DOINTV
   * - :ref:`Reporting - Log Frequency <option-CONOPT-log_frequency>`
     - LFILOG
   * - :ref:`Reporting - Log Frequency SLP and SQP <option-CONOPT-log_frequency_slp_and_sqp>`
     - LFILOS
   * - :ref:`Scaling - Maximal Scaling Factor <option-CONOPT-maximal_scaling_factor>`
     - RTMAXS
   * - :ref:`Scaling - Minimal Jacobian Element for Scaling <option-CONOPT-minimal_jacobian_element_for_scaling>`
     - RTMINJ
   * - :ref:`Scaling - Minimal Scaling Factor <option-CONOPT-minimal_scaling_factor>`
     - RTMINS
   * - :ref:`Scaling - Minimal Scaling Factor 2nd Order Derivatives <option-CONOPT-minimal_scaling_factor_2nd_order_derivatives>`
     - RTMNS2
   * - :ref:`Scaling - Minimal Scaling Tolerance for Variables <option-CONOPT-minimal_scaling_tolerance_for_variables>`
     - RTMINV
   * - :ref:`Scaling - Rescale Frequency <option-CONOPT-rescale_frequency>`
     - LFSCAL
   * - :ref:`Scaling - Scaling Method <option-CONOPT-scaling_method>`
     - LMSCAL
   * - :ref:`Stop criteria - Accuracy One Dimensional Search <option-CONOPT-accuracy_one_dimensional_search>`
     - RTONED
   * - :ref:`Stop criteria - Limit for Slow Progress <option-CONOPT-limit_for_slow_progress>`
     - LFNICR
   * - :ref:`Stop criteria - Maximal Number of Stalled Iterations <option-CONOPT-maximal_number_of_stalled_iterations>`
     - LFSTAL
   * - :ref:`Stop criteria - Optimality Tolerance <option-CONOPT-optimality_tolerance>`
     - RTREDG
   * - :ref:`Stop criteria - Optimality Tolerance Infeasible <option-CONOPT-optimality_tolerance_infeasible>`
     - RTREDI
   * - :ref:`Stop criteria - Slow Progress Tolerance <option-CONOPT-slow_progress_tolerance>`
     - RTOBJL
