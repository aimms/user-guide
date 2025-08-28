

.. _AIMMS_to_GUROBI_Mapping:


AIMMS to GUROBI Mapping
============================

**Description** 

The table shows in the left column the AIMMS Gurobi options while the right column displays the associated Gurobi parameter.

.. list-table::

   * - **Option name in AIMMS** 
     - **Name in GUROBI** 
   * - :ref:`option-GUROBI-barrier_convergence_tolerance` 
     - BARCONVTOL
   * - :ref:`option-GUROBI-barrier_correction_steps` 
     - BARCORRECTORS
   * - :ref:`option-GUROBI-barrier_crossover` 
     - CROSSOVER
   * - :ref:`option-GUROBI-barrier_crossover_basis` 
     - CROSSOVERBASIS
   * - :ref:`option-GUROBI-barrier_homogeneous_algorithm` 
     - BARHOMOGENEOUS
   * - :ref:`option-GUROBI-barrier_iteration_limit` 
     - BARITERLIMIT
   * - :ref:`option-GUROBI-barrier_ordering` 
     - BARORDER
   * - :ref:`option-GUROBI-barrier_progress_solution` 
     - 
   * - :ref:`option-GUROBI-barrier_qcp_convergence_tolerance` 
     - BARQCPCONVTOL
   * - :ref:`option-GUROBI-calculate_kappa` 
     - 
   * - :ref:`option-GUROBI-concurrent_method` 
     - CONCURRENTMETHOD
   * - :ref:`option-GUROBI-farkas_infeasibility_proof`  
     - 
   * - :ref:`option-GUROBI-feasibility`  
     - FEASIBILITYTOL
   * - :ref:`option-GUROBI-iis_method` 
     - FEASRELAXBIGM
   * - :ref:`option-GUROBI-iis_method`  
     - IISMETHOD
   * - :ref:`option-GUROBI-memory_limit` 
     - MEMLIMIT
   * - :ref:`option-GUROBI-method`  
     - METHOD
   * - :ref:`option-GUROBI-mps`  
     - 
   * - :ref:`option-GUROBI-mps_dual` 
     - 
   * - :ref:`option-GUROBI-multi_objective_method`  
     - MULTIOBJMETHOD
   * - :ref:`option-GUROBI-numeric_focus`  
     - NUMERICFOCUS
   * - :ref:`option-GUROBI-optimality`  
     - OPTIMALITYTOL
   * - :ref:`option-GUROBI-random_seed`  
     - SEED
   * - :ref:`option-GUROBI-read_parameter_file`  
     - 
   * - :ref:`option-GUROBI-restart`  
     - 
   * - :ref:`option-GUROBI-restart_file_number` 
     - 
   * - :ref:`option-GUROBI-scale`  
     - SCALEFLAG
   * - :ref:`option-GUROBI-sensitivity_method`  
     - 
   * - :ref:`option-GUROBI-soft_memory_limit` 
     - SOFTMEMLIMIT
   * - :ref:`option-GUROBI-solution_file`  
     - 
   * - :ref:`option-GUROBI-solution_target`  
     - SOLUTIONTARGET
   * - :ref:`option-GUROBI-unbounded_ray`  
     - 
   * - :ref:`option-GUROBI-updates_batch_size`  
     - 
   * - :ref:`option-GUROBI-warm_start` 
     - LPWARMSTART
   * - :ref:`option-GUROBI-work_limit` 
     - WORKLIMIT
   * - :ref:`option-GUROBI-write_parameter_file` 
     - 
   * - :ref:`option-GUROBI-display_solution_quality`  
     - 
   * - :ref:`option-GUROBI-log_to_console`  
     - LOGTOCONSOLE
   * - :ref:`option-GUROBI-output_file`  
     - OUTPUTFLAG
   * - :ref:`option-GUROBI-output_file_display_interval`  
     - DISPLAYINTERVAL
   * - :ref:`option-GUROBI-tune_output_level`  
     - TUNEOUTPUT
   * - :ref:`option-GUROBI-branch_direction`  
     - BRANCHDIR
   * - :ref:`option-GUROBI-disconnected_component_strategy`  
     - DISCONNECTED
   * - :ref:`option-GUROBI-hints_file`  
     - 
   * - :ref:`option-GUROBI-improve_start_gap` 
     - IMPROVESTARTGAP
   * - :ref:`option-GUROBI-improve_start_nodes` 
     - IMPROVESTARTNODES
   * - :ref:`option-GUROBI-improve_start_time` 
     - IMPROVESTARTTIME
   * - :ref:`option-GUROBI-integrality`  
     - INTFEASTOL
   * - :ref:`option-GUROBI-integrality_focus`  
     - INTEGRALITYFOCUS
   * - :ref:`option-GUROBI-lazy_constraint_mode`  
     - 
   * - :ref:`option-GUROBI-mip_best_bound_stop`  
     - BESTBDSTOP
   * - :ref:`option-GUROBI-mip_best_objective_stop`  
     - BESTOBJSTOP
   * - :ref:`option-GUROBI-mip_focus`  
     - MIPFOCUS
   * - :ref:`option-GUROBI-mip_node_method`  
     - NODEMETHOD
   * - :ref:`option-GUROBI-mip_start`  
     - 
   * - :ref:`option-GUROBI-mip_start_node_limit`  
     - STARTNODELIMIT
   * - :ref:`option-GUROBI-mip_symmetry`  
     - SYMMETRY
   * - :ref:`option-GUROBI-node_file_start`  
     - NODEFILESTART
   * - :ref:`option-GUROBI-node_limit`  
     - NODELIMIT
   * - :ref:`option-GUROBI-select_variables`  
     - VARBRANCH
   * - :ref:`option-GUROBI-bqp_cuts` 
     - BQPCUTS
   * - :ref:`option-GUROBI-clique_cuts`  
     - CLIQUECUTS
   * - :ref:`option-GUROBI-cover_cuts` 
     - COVERCUTS
   * - :ref:`option-GUROBI-dual_implied_cuts` 
     - DUALIMPLIEDCUTS
   * - :ref:`option-GUROBI-cut_aggregation_passes_limit` 
     - CUTAGGPASSES
   * - :ref:`option-GUROBI-flow_cover_cuts` 
     - FLOWCOVERCUTS
   * - :ref:`option-GUROBI-flow_path_cuts` 
     - FLOWPATHCUTS
   * - :ref:`option-GUROBI-global_cut_control`  
     - CUTS
   * - :ref:`option-GUROBI-gomory_cut_passes_limit` 
     - GOMORYPASSES
   * - :ref:`option-GUROBI-gub_cover_cuts` 
     - GUBCOVERCUTS
   * - :ref:`option-GUROBI-implied_bound_cuts` 
     - IMPLIEDCUTS
   * - :ref:`option-GUROBI-infeasibility_proof_cuts` 
     - INFPROOFCUTS
   * - :ref:`option-GUROBI-lift_and_project_cuts`  
     - LIFTPROJECTCUTS
   * - :ref:`option-GUROBI-mip_separation_cuts`  
     - MIPSEPCUTS
   * - :ref:`option-GUROBI-mir_cuts`  
     - MIRCUTS
   * - :ref:`option-GUROBI-mixing_cuts`  
     - MIXINGCUTS
   * - :ref:`option-GUROBI-mod_k_cuts`  
     - MODKCUTS
   * - :ref:`option-GUROBI-network_cuts`  
     - NETWORKCUTS
   * - :ref:`option-GUROBI-projected_implied_bound_cuts` 
     - PROJIMPLIEDCUTS
   * - :ref:`option-GUROBI-relax-and-lift_cuts`  
     - RELAXLIFTCUTS
   * - :ref:`option-GUROBI-rlt_cuts` 
     - RLTCUTS
   * - :ref:`option-GUROBI-root_cut_passes_limit` 
     - CUTPASSES
   * - :ref:`option-GUROBI-strong_cg_cuts`  
     - STRONGCGCUTS
   * - :ref:`option-GUROBI-sub_mip_cuts`  
     - SUBMIPCUTS
   * - :ref:`option-GUROBI-zero_half_cuts`  
     - ZEROHALFCUTS
   * - :ref:`option-GUROBI-feasibility_pump_passes` 
     - PUMPPASSES
   * - :ref:`option-GUROBI-heuristics`  
     - HEURISTICS
   * - :ref:`option-GUROBI-minimum_relaxation_heuristic_node_limit` 
     - MINRELNODES
   * - :ref:`option-GUROBI-no_relaxation_heuristic_time` 
     - NORELHEURTIME
   * - :ref:`option-GUROBI-no_relaxation_heuristic_work` 
     - NORELHEURWORK
   * - :ref:`option-GUROBI-partition_heuristic`  
     - PARTITIONPLACE
   * - :ref:`option-GUROBI-rins_heuristic_frequency`  
     - RINS
   * - :ref:`option-GUROBI-rins_sub_mip_node_limit`  
     - SUBMIPNODES
   * - :ref:`option-GUROBI-zero_objective_node_limit` 
     - ZEROOBJNODES
   * - :ref:`option-GUROBI-mip_obbt` 
     - OBBT
   * - :ref:`option-GUROBI-presolve_sparsify_reduction` 
     - PRESPARSIFY
   * - :ref:`option-GUROBI-sos1_encoding` 
     - PRESOS1ENCODING
   * - :ref:`option-GUROBI-sos1_reformulation_threshold` 
     - PRESOS1BIGM
   * - :ref:`option-GUROBI-sos2_encoding` 
     - PRESOS2ENCODING
   * - :ref:`option-GUROBI-sos2_reformulation_threshold` 
     - PRESOS2BIGM
   * - :ref:`option-GUROBI-maximal_variable_bound` 
     - 
   * - :ref:`option-GUROBI-nonlinear_optimality_tolerance` 
     - MIPGAP
   * - :ref:`option-GUROBI-concurrent_mip` 
     - CONCURRENTMIP
   * - :ref:`option-GUROBI-thread_limit` 
     - THREADS
   * - :ref:`option-GUROBI-dual_reductions` 
     - DUALREDUCTIONS
   * - :ref:`option-GUROBI-linearize_quadratic_constraints` 
     - PREQLINEARIZE
   * - :ref:`option-GUROBI-multi_objective_presolve`  
     - MULTIOBJPRE
   * - :ref:`option-GUROBI-presolve` 
     - PRESOLVE
   * - :ref:`option-GUROBI-presolve_aggregation`  
     - AGGREGATE
   * - :ref:`option-GUROBI-presolve_aggregation_fill`  
     - AGGFILL
   * - :ref:`option-GUROBI-presolve_dual` 
     - PREDUAL
   * - :ref:`option-GUROBI-presolve_passes` 
     - PREPASSES
   * - :ref:`option-GUROBI-presolve_row_reduction` 
     - PREDEPROW
   * - :ref:`option-GUROBI-miqcp_formulation` 
     - PREMIQCPFORM
   * - :ref:`option-GUROBI-miqcp_method` 
     - MIQCPMETHOD
   * - :ref:`option-GUROBI-nlp_heuristic` 
     - NLPHEUR
   * - :ref:`option-GUROBI-nonconvex_strategy` 
     - NONCONVEX
   * - :ref:`option-GUROBI-psd_tolerance` 
     - PSDTOL
   * - :ref:`option-GUROBI-qcp_dual_values` 
     - QCPDUAL
   * - :ref:`option-GUROBI-degenerate_simplex_moves_limit` 
     - DEGENMOVES
   * - :ref:`option-GUROBI-markowitz` 
     - MARKOWITZTOL	
   * - :ref:`option-GUROBI-network_algorithm` 
     - NETWORKALG
   * - :ref:`option-GUROBI-norm_adjust` 
     - NORMADJUST
   * - :ref:`option-GUROBI-objective_scale` 
     - OBJSCALE
   * - :ref:`option-GUROBI-perturbation` 
     - PERTURBVALUE
   * - :ref:`option-GUROBI-pricing`  
     - SIMPLEXPRICING
   * - :ref:`option-GUROBI-quad_precision`  
     - QUAD
   * - :ref:`option-GUROBI-sifting` 
     - SIFTING
   * - :ref:`option-GUROBI-sifting_method` 
     - SIFTMETHOD
   * - :ref:`option-GUROBI-pool_absolute_gap` 
     - POOLGAPABS
   * - :ref:`option-GUROBI-pool_gap` 
     - POOLGAP
   * - :ref:`option-GUROBI-pool_search_mode` 
     - POOLSEARCHMODE
   * - :ref:`option-GUROBI-pool_size` 
     - POOLSOLUTIONS
   * - :ref:`option-GUROBI-tune_cleanup` 
     - TUNECLEANUP
   * - :ref:`option-GUROBI-tune_criterion` 
     - TUNECRITERION
   * - :ref:`option-GUROBI-tune_metric` 
     - TUNEMETRIC
   * - :ref:`option-GUROBI-tune_results` 
     - TUNERESULTS
   * - :ref:`option-GUROBI-tune_target_mip_gap` 
     - TUNETARGETMIPGAP
   * - :ref:`option-GUROBI-tune_target_time` 
     - TUNETARGETTIME
   * - :ref:`option-GUROBI-tune_time_limit` 
     - TUNETIMELIMIT
   * - :ref:`option-GUROBI-tune_trials`  
     - TUNETRIALS


The table below shows Solvers General options that are mapped to Gurobi parameters.

.. list-table::

   * - **Option name in AIMMS** 
     - **Name in GUROBI** 
   * - :ref:`option-AIMMS-cutoff` 
     - CUTOFF
   * - :ref:`option-AIMMS-maximal_number_of_integer_solutions` 
     - SOLUTIONLIMIT
   * - :ref:`option-AIMMS-mip_absolute_optimality_tolerance` 
     - MIPGAPABS
   * - :ref:`option-AIMMS-mip_relative_optimality_tolerance` 
     - MIPGAP
   * - :ref:`option-AIMMS-iteration_limit` 
     - ITERATIONLIMIT
   * - :ref:`option-AIMMS-time_limit` 
     - TIMELIMIT


