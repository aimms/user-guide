

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
   * - :ref:`option-CONOPT-box_size_factor_linear_variables`
     - RTBOXF
   * - :ref:`option-CONOPT-box_size_tolerance`
     - RTBOX
   * - :ref:`option-CONOPT-box_size_tolerance_linear`
     - RTBOXL
   * - :ref:`option-CONOPT-fixed_variables_tolerance_derived_bounds`
     - RTBNDT
   * - :ref:`option-CONOPT-fixed_variables_tolerance_initial_bounds`
     - RTBNDI
   * - :ref:`option-CONOPT-logical_switch_for_selection_of_slacks`
     - LSLACK
   * - :ref:`option-CONOPT-method_for_defined_variables`
     - LMUSDF
   * - :ref:`option-CONOPT-method_for_finding_maximal_step`
     - LMMXSF
   * - :ref:`option-CONOPT-method_for_finding_maximal_tight_step`
     - LMMXST
   * - :ref:`option-CONOPT-method_for_linear_feasibility_models`
     - LMETHOD
   * - :ref:`option-CONOPT-method_for_reduced_hessian`
     - LMNDIA
   * - :ref:`option-CONOPT-penalty_constraints_ratio`
     - RTNOPN
   * - :ref:`option-CONOPT-relative_objective_accuracy`
     - RTOBJR
   * - :ref:`option-CONOPT-slp_mode`
     - LSESLP
   * - :ref:`option-CONOPT-sqp_mode`
     - LSESQP
   * - :ref:`option-CONOPT-steplength_multiplier`
     - RVSTLM
   * - :ref:`option-CONOPT-use_no-penalty_model`
     - DONOPEN
   * - :ref:`option-CONOPT-zero_filter_tolerance_jacobian_elements`
     - RTMINA
   * - :ref:`option-CONOPT-check_1st_order_derivatives`
     - LKDEBG
   * - :ref:`option-CONOPT-check_2nd_order_derivatives`
     - LKDEB2
   * - :ref:`option-CONOPT-tolerance_2nd_order_derivatives_check`
     - RT2DRV
   * - :ref:`option-CONOPT-bound_tolerance`
     - RTBND1
   * - :ref:`option-CONOPT-feasibility_tolerance_triangular_part`
     - RTNWTR
   * - :ref:`option-CONOPT-maximal_feasibility_tolerance`
     - RTNWMA
   * - :ref:`option-CONOPT-method_for_initial_basis`
     - LSCRSH
   * - :ref:`option-CONOPT-minimal_feasibility_tolerance`
     - RTNWMI
   * - :ref:`option-CONOPT-model_is_convex`
     - ISCONVEX
   * - :ref:`option-CONOPT-model_is_square_system`
     - LSSQRS
   * - :ref:`option-CONOPT-limit_on_candidates_for_defined_variable`
     - LFUSDF
   * - :ref:`option-CONOPT-limit_on_degenerate_iterations`
     - LFDEGI
   * - :ref:`option-CONOPT-limit_on_directional_2nd_order_derivative_errors`
     - LF2DRV
   * - :ref:`option-CONOPT-limit_on_hessian_evaluation_errors`
     - LFHSOK
   * - :ref:`option-CONOPT-limit_on_linear_feasibility_model_rounds`
     - NROUNDS
   * - :ref:`option-CONOPT-limit_on_new_superbasics`
     - LFMXNS
   * - :ref:`option-CONOPT-maximal_hessian_dimension`
     - LFNSUP
   * - :ref:`option-CONOPT-maximum_solution_of_a_variable`
     - RTMAXV
   * - :ref:`option-CONOPT-absolute_pivot_tolerance`
     - RTPIVA
   * - :ref:`option-CONOPT-absolute_pivot_tolerance_initial_basis`
     - RTIPVA
   * - :ref:`option-CONOPT-absolute_pivot_tolerance_nonlinear_elements`
     - RTPIVT
   * - :ref:`option-CONOPT-relative_pivot_tolerance`
     - RTPIVR
   * - :ref:`option-CONOPT-relative_pivot_tolerance_during_basis_updates`
     - RTPIVU
   * - :ref:`option-CONOPT-relative_pivot_tolerance_during_ratio_test`
     - RTPIVS
   * - :ref:`option-CONOPT-relative_pivot_tolerance_during_basis_updates`
     - RTIPVR
   * - :ref:`option-CONOPT-preprocessor`
     - DOPREP
   * - :ref:`option-CONOPT-use_interval_evaluations`
     - DOINTV
   * - :ref:`option-CONOPT-log_frequency`
     - LFILOG
   * - :ref:`option-CONOPT-log_frequency_slp_and_sqp`
     - LFILOS
   * - :ref:`option-CONOPT-maximal_scaling_factor`
     - RTMAXS
   * - :ref:`option-CONOPT-minimal_jacobian_element_for_scaling`
     - RTMINJ
   * - :ref:`option-CONOPT-minimal_scaling_factor`
     - RTMINS
   * - :ref:`option-CONOPT-minimal_scaling_factor_2nd_order_derivatives`
     - RTMNS2
   * - :ref:`option-CONOPT-minimal_scaling_tolerance_for_variables`
     - RTMINV
   * - :ref:`option-CONOPT-rescale_frequency`
     - LFSCAL
   * - :ref:`option-CONOPT-scaling_method`
     - LMSCAL
   * - :ref:`option-CONOPT-accuracy_one_dimensional_search`
     - RTONED
   * - :ref:`option-CONOPT-limit_for_slow_progress`
     - LFNICR
   * - :ref:`option-CONOPT-maximal_number_of_stalled_iterations`
     - LFSTAL
   * - :ref:`option-CONOPT-optimality_tolerance`
     - RTREDG
   * - :ref:`option-CONOPT-optimality_tolerance_infeasible`
     - RTREDI
   * - :ref:`option-CONOPT-slow_progress_tolerance`
     - RTOBJL
