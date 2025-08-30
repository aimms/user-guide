

.. _GUROBI_to_AIMMS_Mapping:


Gurobi to AIMMS Mapping
============================

**Description** 

The table shows in the left column the parameters from Gurobi that can be set in AIMMS; 
the right column displays for each Gurobi parameter the associated AIMMS option.

.. list-table::

   * - **Name in Gurobi**
     - **Option name in AIMMS**
   * - AGGFILL
     - :ref:`option-GUROBI-presolve_aggregation_fill`
   * - AGGREGATE
     - :ref:`option-GUROBI-presolve_aggregation`
   * - BARCONVTOL
     - :ref:`option-GUROBI-barrier_convergence_tolerance`
   * - BARCORRECTORS
     - :ref:`option-GUROBI-barrier_correction_steps`
   * - BARHOMOGENEOUS
     - :ref:`option-GUROBI-barrier_homogeneous_algorithm`
   * - BARITERLIMIT
     - :ref:`option-GUROBI-barrier_iteration_limit`
   * - BARORDER
     - :ref:`option-GUROBI-barrier_ordering`
   * - BARQCPCONVTOL
     - :ref:`option-GUROBI-barrier_qcp_convergence_tolerance`
   * - BESTBDSTOP
     - :ref:`option-GUROBI-mip_best_bound_stop`
   * - BESTOBJSTOP
     - :ref:`option-GUROBI-mip_best_objective_stop`
   * - BQPCUTS
     - :ref:`option-GUROBI-bqp_cuts`
   * - BRANCHDIR
     - :ref:`option-GUROBI-branch_direction`
   * - CLIQUECUTS
     - :ref:`option-GUROBI-clique_cuts`
   * - CONCURRENTMETHOD
     - :ref:`option-GUROBI-concurrent_method`
   * - CONCURRENTMIP
     - :ref:`option-GUROBI-concurrent_mip`
   * - COVERCUTS
     - :ref:`option-GUROBI-cover_cuts`
   * - CROSSOVER
     - :ref:`option-GUROBI-barrier_crossover`
   * - CROSSOVERBASIS
     - :ref:`option-GUROBI-barrier_crossover_basis`
   * - CUTAGGPASSES
     - :ref:`option-GUROBI-cut_aggregation_passes_limit`
   * - CUTPASSES
     - :ref:`option-GUROBI-root_cut_passes_limit`
   * - CUTS
     - :ref:`option-GUROBI-global_cut_control`
   * - DEGENMOVES
     - :ref:`option-GUROBI-degenerate_simplex_moves_limit`
   * - DISCONNECTED
     - :ref:`option-GUROBI-disconnected_component_strategy`
   * - DISPLAYINTERVAL
     - :ref:`option-GUROBI-output_file_display_interval`
   * - DUALIMPLIEDCUTS
     - :ref:`option-GUROBI-dual_implied_cuts`
   * - DUALREDUCTIONS
     - :ref:`option-GUROBI-dual_reductions`
   * - FEASIBILITYTOL
     - :ref:`option-GUROBI-feasibility`
   * - FEASRELAXBIGM
     - :ref:`option-GUROBI-feasrelax_big_m`
   * - FLOWCOVERCUTS
     - :ref:`option-GUROBI-flow_cover_cuts`
   * - FLOWPATHCUTS
     - :ref:`option-GUROBI-flow_path_cuts`
   * - GOMORYPASSES
     - :ref:`option-GUROBI-gomory_cut_passes_limit`
   * - GUBCOVERCUTS
     - :ref:`option-GUROBI-gub_cover_cuts`
   * - HEURISTICS
     - :ref:`option-GUROBI-heuristics`
   * - IISMETHOD
     - :ref:`option-GUROBI-iis_method`
   * - IMPLIEDCUTS
     - :ref:`option-GUROBI-implied_bound_cuts`
   * - IMPROVESTARTGAP
     - :ref:`option-GUROBI-improve_start_gap`
   * - IMPROVESTARTNODES
     - :ref:`option-GUROBI-improve_start_nodes`
   * - IMPROVESTARTTIME
     - :ref:`option-GUROBI-improve_start_time`
   * - INFPROOFCUTS
     - :ref:`option-GUROBI-infeasibility_proof_cuts`
   * - INTEGRALITYFOCUS
     - :ref:`option-GUROBI-integrality_focus`
   * - INTFEASTOL
     - :ref:`option-GUROBI-integrality`
   * - LIFTPROJECTCUTS
     - :ref:`option-GUROBI-lift_and_project_cuts`
   * - LOGTOCONSOLE
     - :ref:`option-GUROBI-log_to_console`
   * - LPWARMSTART
     - :ref:`option-GUROBI-warm_start`
   * - MARKOWITZTOL
     - :ref:`option-GUROBI-markowitz`
   * - MEMLIMIT
     - :ref:`option-GUROBI-memory_limit`
   * - METHOD
     - :ref:`option-GUROBI-method`
   * - MINRELNODES
     - :ref:`option-GUROBI-minimum_relaxation_heuristic_node_limit`
   * - MIPFOCUS
     - :ref:`option-GUROBI-mip_focus`
   * - MIPSEPCUTS
     - :ref:`option-GUROBI-mip_separation_cuts`
   * - MIQCPMETHOD
     - :ref:`option-GUROBI-miqcp_method`
   * - MIRCUTS
     - :ref:`option-GUROBI-mir_cuts`
   * - MIXINGCUTS
     - :ref:`option-GUROBI-mixing_cuts`
   * - MODKCUTS
     - :ref:`option-GUROBI-mod_k_cuts`
   * - MULTIOBJMETHOD
     - :ref:`option-GUROBI-multi_objective_method`
   * - MULTIOBJPRE
     - :ref:`option-GUROBI-multi_objective_presolve`
   * - NETWORKALG
     - :ref:`option-GUROBI-network_algorithm`
   * - NETWORKCUTS
     - :ref:`option-GUROBI-network_cuts`
   * - NLPHEUR
     - :ref:`option-GUROBI-nlp_heuristic`
   * - NODEFILESTART
     - :ref:`option-GUROBI-node_file_start`
   * - NODELIMIT
     - :ref:`option-GUROBI-node_limit`
   * - NODEMETHOD
     - :ref:`option-GUROBI-mip_node_method`
   * - NONCONVEX
     - :ref:`option-GUROBI-nonconvex_strategy`
   * - NORELHEURTIME
     - :ref:`option-GUROBI-no_relaxation_heuristic_time`
   * - NORELHEURWORK
     - :ref:`option-GUROBI-no_relaxation_heuristic_work`
   * - NORMADJUST
     - :ref:`option-GUROBI-norm_adjust`
   * - NUMERICFOCUS
     - :ref:`option-GUROBI-numeric_focus`
   * - OBBT
     - :ref:`option-GUROBI-mip_obbt`
   * - OBJSCALE
     - :ref:`option-GUROBI-objective_scale`
   * - OPTIMALITYTOL
     - :ref:`option-GUROBI-optimality`
   * - OUTPUTFLAG
     - :ref:`option-GUROBI-output_file`
   * - PARTITIONPLACE
     - :ref:`option-GUROBI-partition_heuristic`
   * - PERTURBVALUE
     - :ref:`option-GUROBI-perturbation`
   * - POOLGAP
     - :ref:`option-GUROBI-pool_gap`
   * - POOLGAPABS
     - :ref:`option-GUROBI-pool_absolute_gap`
   * - POOLSEARCHMODE
     - :ref:`option-GUROBI-pool_search_mode`
   * - POOLSOLUTIONS
     - :ref:`option-GUROBI-pool_size`
   * - PREDEPROW
     - :ref:`option-GUROBI-presolve_row_reduction`
   * - PREDUAL
     - :ref:`option-GUROBI-presolve_dual`
   * - PREMIQCPFORM
     - :ref:`option-GUROBI-miqcp_formulation`
   * - PREPASSES
     - :ref:`option-GUROBI-presolve_passes`
   * - PREQLINEARIZE
     - :ref:`option-GUROBI-linearize_quadratic_constraints`
   * - PRESOLVE
     - :ref:`option-GUROBI-presolve`
   * - PRESOS1BIGM
     - :ref:`option-GUROBI-sos1_reformulation_threshold`
   * - PRESOS1ENCODING
     - :ref:`option-GUROBI-sos1_encoding`
   * - PRESOS2BIGM
     - :ref:`option-GUROBI-sos2_reformulation_threshold`
   * - PRESOS2ENCODING
     - :ref:`option-GUROBI-sos2_encoding`
   * - PRESPARSIFY
     - :ref:`option-GUROBI-presolve_sparsify_reduction`
   * - PROJIMPLIEDCUTS
     - :ref:`option-GUROBI-projected_implied_bound_cuts`
   * - PSDTOL
     - :ref:`option-GUROBI-psd_tolerance`
   * - PUMPPASSES
     - :ref:`option-GUROBI-feasibility_pump_passes`
   * - QCPDUAL
     - :ref:`option-GUROBI-qcp_dual_values`
   * - QUAD
     - :ref:`option-GUROBI-quad_precision`
   * - RELAXLIFTCUTS
     - :ref:`option-GUROBI-relax-and-lift_cuts`
   * - RINS
     - :ref:`option-GUROBI-rins_heuristic_frequency`
   * - RLTCUTS
     - :ref:`option-GUROBI-rlt_cuts`
   * - SCALEFLAG
     - :ref:`option-GUROBI-scale`
   * - SEED
     - :ref:`option-GUROBI-random_seed`
   * - SIFTING
     - :ref:`option-GUROBI-sifting`
   * - SIFTMETHOD
     - :ref:`option-GUROBI-sifting_method`
   * - SIMPLEXPRICING
     - :ref:`option-GUROBI-pricing`
   * - SOFTMEMLIMIT
     - :ref:`option-GUROBI-soft_memory_limit`
   * - SOLUTIONTARGET
     - :ref:`option-GUROBI-solution_target`
   * - STARTNODELIMIT
     - :ref:`option-GUROBI-mip_start_node_limit`
   * - STRONGCGCUTS
     - :ref:`option-GUROBI-strong_cg_cuts`
   * - SUBMIPCUTS
     - :ref:`option-GUROBI-sub_mip_cuts`
   * - SUBMIPNODES
     - :ref:`option-GUROBI-rins_sub_mip_node_limit`
   * - SYMMETRY
     - :ref:`option-GUROBI-mip_symmetry`
   * - THREADS
     - :ref:`option-GUROBI-thread_limit`
   * - TUNECLEANUP
     - :ref:`option-GUROBI-tune_cleanup`
   * - TUNECRITERION
     - :ref:`option-GUROBI-tune_criterion`
   * - TUNEMETRIC
     - :ref:`option-GUROBI-tune_metric`
   * - TUNEOUTPUT
     - :ref:`option-GUROBI-tune_output_level`
   * - TUNERESULTS
     - :ref:`option-GUROBI-tune_results`
   * - TUNETARGETMIPGAP
     - :ref:`option-GUROBI-tune_target_mip_gap`
   * - TUNETARGETTIME
     - :ref:`option-GUROBI-tune_target_time`
   * - TUNETIMELIMIT
     - :ref:`option-GUROBI-tune_time_limit`
   * - TUNETRIALS
     - :ref:`option-GUROBI-tune_trials`
   * - VARBRANCH
     - :ref:`option-GUROBI-select_variables`
   * - WORKLIMIT
     - :ref:`option-GUROBI-work_limit`
   * - ZEROHALFCUTS
     - :ref:`option-GUROBI-zero_half_cuts`
   * - ZEROOBJNODES
     - :ref:`option-GUROBI-zero_objective_node_limit`


**Note** 

*	The Gurobi parameter PRECRUSH is not available in AIMMS. AIMMS automatically switches it on when a cut callback procedure is installed in the AIMMS model.
