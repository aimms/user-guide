.. _CONOPT_to_AIMMS_Mapping:


CONOPT to AIMMS Mapping
=======================

**Description** 

The table shows in the left column the parameters from CONOPT that can be set in AIMMS; the right column displays for each CONOPT parameter the associated AIMMS option.
	
.. list-table::

   * - **Name in CONOPT**
     - **Option name in AIMMS**
   * - DOINTV
     - :ref:`option-CONOPT-use_interval_evaluations`
   * - DONOPEN
     - :ref:`option-CONOPT-use_no-penalty_model`
   * - DOPREP
     - :ref:`option-CONOPT-preprocessor`
   * - LF2DRV
     - :ref:`option-CONOPT-limit_on_directional_2nd_order_derivative_errors`
   * - LFDEGI
     - :ref:`option-CONOPT-limit_on_degenerate_iterations`
   * - LFHSOK
     - :ref:`option-CONOPT-limit_on_hessian_evaluation_errors`
   * - LFILOG
     - :ref:`option-CONOPT-log_frequency`
   * - LFILOS
     - :ref:`option-CONOPT-log_frequency_slp_and_sqp`
   * - LFITER
     - :ref:`Options_Stop_Criteria_-_Iteration_Limi`  in 'Solvers - General'
   * - LFMXNS
     - :ref:`option-CONOPT-limit_on_new_superbasics`
   * - LFNICR
     - :ref:`option-CONOPT-limit_for_slow_progress`
   * - LFNSUP
     - :ref:`option-CONOPT-maximal_hessian_dimension`
   * - LFSCAL
     - :ref:`option-CONOPT-rescale_frequency`
   * - LFSTAL
     - :ref:`option-CONOPT-maximal_number_of_stalled_iterations`
   * - LFUSDF
     - :ref:`option-CONOPT-limit_on_candidates_for_defined_variable`
   * - LKDEB2
     - :ref:`option-CONOPT-check_2nd_order_derivatives`
   * - LKDEBG
     - :ref:`option-CONOPT-check_1st_order_derivatives`
   * - LMETHOD
     - :ref:`option-CONOPT-method_for_linear_feasibility_models`
   * - LMMXSF
     - :ref:`option-CONOPT-method_for_finding_maximal_step`
   * - LMMXST
     - :ref:`option-CONOPT-method_for_finding_maximal_tight_step`
   * - LMNDIA
     - :ref:`option-CONOPT-method_for_reduced_hessian`
   * - LMSCAL
     - :ref:`option-CONOPT-scaling_method`
   * - LMUSDF
     - :ref:`option-CONOPT-method_for_defined_variables`
   * - LSCRSH
     - :ref:`option-CONOPT-method_for_initial_basis`
   * - LSESLP
     - :ref:`option-CONOPT-slp_mode`
   * - LSESQP
     - :ref:`option-CONOPT-sqp_mode`
   * - LSLACK
     - :ref:`option-CONOPT-logical_switch_for_selection_of_slacks`
   * - LSSQRS
     - :ref:`option-CONOPT-model_is_square_system`
   * - ISCONVEX
     - :ref:`option-CONOPT-model_is_convex`
   * - NROUNDS
     - :ref:`option-CONOPT-limit_on_linear_feasibility_model_rounds`
   * - RT2DRV
     - :ref:`option-CONOPT-tolerance_2nd_order_derivatives_check`
   * - RTBND1
     - :ref:`option-CONOPT-bound_tolerance`
   * - RTBNDI
     - :ref:`option-CONOPT-fixed_variables_tolerance_initial_bounds`
   * - RTBNDT
     - :ref:`option-CONOPT-fixed_variables_tolerance_derived_bounds`
   * - RTBOX
     - :ref:`option-CONOPT-box_size_tolerance`
   * - RTBOXF
     - :ref:`option-CONOPT-box_size_factor_linear_variables`
   * - RTBOXL
     - :ref:`option-CONOPT-box_size_tolerance_linear`
   * - RTIPVA
     - :ref:`option-CONOPT-absolute_pivot_tolerance_initial_basis`
   * - RTIPVR
     - :ref:`option-CONOPT-relative_pivot_tolerance_initial_basis`
   * - RTMAXS
     - :ref:`option-CONOPT-maximal_scaling_factor`
   * - RTMAXV
     - :ref:`option-CONOPT-maximum_solution_of_a_variable`
   * - RTMINA
     - :ref:`option-CONOPT-zero_filter_tolerance_jacobian_elements`
   * - RTMINJ
     - :ref:`option-CONOPT-minimal_jacobian_element_for_scaling`
   * - RTMINS
     - :ref:`option-CONOPT-minimal_scaling_factor`
   * - RTMINV
     - :ref:`option-CONOPT-minimal_scaling_tolerance_for_variables`
   * - RTMNS2
     - :ref:`option-CONOPT-minimal_scaling_factor_2nd_order_derivatives`
   * - RTNOPN
     - :ref:`option-CONOPT-penalty_constraints_ratio`
   * - RTNWMA
     - :ref:`option-CONOPT-maximal_feasibility_tolerance`
   * - RTNWMI
     - :ref:`option-CONOPT-minimal_feasibility_tolerance`
   * - RTNWTR
     - :ref:`option-CONOPT-feasibility_tolerance_triangular_part`
   * - RTOBJL
     - :ref:`option-CONOPT-slow_progress_tolerance`
   * - RTOBJR
     - :ref:`option-CONOPT-relative_objective_accuracy`
   * - RTONED
     - :ref:`option-CONOPT-accuracy_one_dimensional_search`
   * - RTPIVA
     - :ref:`option-CONOPT-absolute_pivot_tolerance`
   * - RTPIVR
     - :ref:`option-CONOPT-relative_pivot_tolerance`
   * - RTPIVS
     - :ref:`option-CONOPT-relative_pivot_tolerance_during_ratio_test`
   * - RTPIVT
     - :ref:`option-CONOPT-absolute_pivot_tolerance_nonlinear_elements`
   * - RTPIVU
     - :ref:`option-CONOPT-relative_pivot_tolerance_during_basis_updates`
   * - RTREDG
     - :ref:`option-CONOPT-optimality_tolerance`
   * - RTREDI
     - :ref:`option-CONOPT-optimality_tolerance_infeasible`
   * - RVSTLM
     - :ref:`option-CONOPT-steplength_multiplier`
   * - RVTIME
     - :ref:`Options_Stop_Criteria_-_Time_Limit`  in 'Solvers - General'
