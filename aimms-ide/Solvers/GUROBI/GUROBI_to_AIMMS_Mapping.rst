

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
     - :ref:`Presolve - Presolve Aggregation Fill <option-GUROBI-presolve_aggregation_fill>`
   * - AGGREGATE
     - :ref:`Presolve - Presolve Aggregation <option-GUROBI-presolve_aggregation>`
   * - BARCONVTOL
     - :ref:`Barrier - Barrier Convergence Tolerance <option-GUROBI-barrier_convergence_tolerance>`
   * - BARCORRECTORS
     - :ref:`Barrier - Barrier Correction Steps <option-GUROBI-barrier_correction_steps>`
   * - BARHOMOGENEOUS
     - :ref:`Barrier - Barrier Homogeneous Algorithm <option-GUROBI-barrier_homogeneous_algorithm>`
   * - BARITERLIMIT
     - :ref:`Barrier - Barrier Iteration Limit <option-GUROBI-barrier_iteration_limit>`
   * - BARORDER
     - :ref:`Barrier - Barrier Ordering <option-GUROBI-barrier_ordering>`
   * - BARQCPCONVTOL
     - :ref:`Barrier - Barrier QCP Convergence Tolerance <option-GUROBI-barrier_qcp_convergence_tolerance>`
   * - BESTBDSTOP
     - :ref:`MIP - MIP Best Bound Stop <option-GUROBI-mip_best_bound_stop>`
   * - BESTOBJSTOP
     - :ref:`MIP - MIP Best Objective Stop <option-GUROBI-mip_best_objective_stop>`
   * - BQPCUTS
     - :ref:`MIP Cuts - BQP Cuts <option-GUROBI-bqp_cuts>`
   * - BRANCHDIR
     - :ref:`MIP - Branch Direction <option-GUROBI-branch_direction>`
   * - CLIQUECUTS
     - :ref:`MIP Cuts - Clique Cuts <option-GUROBI-clique_cuts>`
   * - CONCURRENTMETHOD
     - :ref:`General - Concurrent Method <option-GUROBI-concurrent_method>`
   * - CONCURRENTMIP
     - :ref:`Parallel - Concurrent MIP <option-GUROBI-concurrent_mip>`
   * - COVERCUTS
     - :ref:`MIP Cuts - Cover Cuts <option-GUROBI-cover_cuts>`
   * - CROSSOVER
     - :ref:`Barrier - Barrier Crossover <option-GUROBI-barrier_crossover>`
   * - CROSSOVERBASIS
     - :ref:`Barrier - Barrier Crossover Basis <option-GUROBI-barrier_crossover_basis>`
   * - CUTAGGPASSES
     - :ref:`MIP Cuts - Cut Aggregation Passes Limit <option-GUROBI-cut_aggregation_passes_limit>`
   * - CUTPASSES
     - :ref:`MIP Cuts - Root Cut Passes Limit <option-GUROBI-root_cut_passes_limit>`
   * - CUTS
     - :ref:`MIP Cuts - Global Cut Control <option-GUROBI-global_cut_control>`
   * - DEGENMOVES
     - :ref:`Simplex - Degenerate Simplex Moves Limit <option-GUROBI-degenerate_simplex_moves_limit>`
   * - DISCONNECTED
     - :ref:`MIP - Disconnected Component Strategy <option-GUROBI-disconnected_component_strategy>`
   * - DISPLAYINTERVAL
     - :ref:`Logging - Output File Display Interval <option-GUROBI-output_file_display_interval>`
   * - DUALIMPLIEDCUTS
     - :ref:`MIP Cuts - Dual Implied Cuts <option-GUROBI-dual_implied_cuts>`
   * - DUALREDUCTIONS
     - :ref:`Presolve - Dual Reductions <option-GUROBI-dual_reductions>`
   * - FEASIBILITYTOL
     - :ref:`General - Feasibility Tolerance <option-GUROBI-feasibility>`
   * - FEASRELAXBIGM
     - :ref:`General - FeasRelax Big M <option-GUROBI-feasrelax_big_m>`
   * - FLOWCOVERCUTS
     - :ref:`MIP Cuts - Flow Cover Cuts <option-GUROBI-flow_cover_cuts>`
   * - FLOWPATHCUTS
     - :ref:`MIP Cuts - Flow Path Cuts <option-GUROBI-flow_path_cuts>`
   * - GOMORYPASSES
     - :ref:`MIP Cuts - Gomory Cut Passes Limit <option-GUROBI-gomory_cut_passes_limit>`
   * - GUBCOVERCUTS
     - :ref:`MIP Cuts - GUB Cover Cuts <option-GUROBI-gub_cover_cuts>`
   * - HEURISTICS
     - :ref:`MIP Heuristics - Heuristics <option-GUROBI-heuristics>`
   * - IISMETHOD
     - :ref:`General - IIS Method <option-GUROBI-iis_method>`
   * - IMPLIEDCUTS
     - :ref:`MIP Cuts - Implied Bound Cuts <option-GUROBI-implied_bound_cuts>`
   * - IMPROVESTARTGAP
     - :ref:`MIP - Improve Start Gap <option-GUROBI-improve_start_gap>`
   * - IMPROVESTARTNODES
     - :ref:`MIP - Improve Start Nodes <option-GUROBI-improve_start_nodes>`
   * - IMPROVESTARTTIME
     - :ref:`MIP - Improve Start Time <option-GUROBI-improve_start_time>`
   * - IMPROVESTARTWORK
     - :ref:`MIP - Improve Start Work <option-GUROBI-improve_start_work>`
   * - INFPROOFCUTS
     - :ref:`MIP Cuts - Infeasibility Proof Cuts <option-GUROBI-infeasibility_proof_cuts>`
   * - INTEGRALITYFOCUS
     - :ref:`MIP - Integrality Focus <option-GUROBI-integrality_focus>`
   * - INTFEASTOL
     - :ref:`MIP - Integrality Tolerance <option-GUROBI-integrality>`
   * - LIFTPROJECTCUTS
     - :ref:`MIP Cuts - Lift and Project Cuts <option-GUROBI-lift_and_project_cuts>`
   * - LOGTOCONSOLE
     - :ref:`Logging - Log to Console <option-GUROBI-log_to_console>`
   * - LPWARMSTART
     - :ref:`General - Warm Start <option-GUROBI-warm_start>`
   * - MARKOWITZTOL
     - :ref:`Simplex - Markowitz Tolerance <option-GUROBI-markowitz>`
   * - MASTERKNAPSACKCUTS
     - :ref:`MIP Cuts - Master Knapsack Cuts <option-GUROBI-master_knapsack_cuts>`
   * - MEMLIMIT
     - :ref:`General - Memory Limit <option-GUROBI-memory_limit>`
   * - METHOD
     - :ref:`General - Method <option-GUROBI-method>`
   * - MINRELNODES
     - :ref:`MIP Heuristics - Minimum Relaxation Heuristic Node Limit <option-GUROBI-minimum_relaxation_heuristic_node_limit>`
   * - MIPFOCUS
     - :ref:`MIP - MIP Focus <option-GUROBI-mip_focus>`
   * - MIPSEPCUTS
     - :ref:`MIP Cuts - MIP Separation Cuts <option-GUROBI-mip_separation_cuts>`
   * - MIQCPMETHOD
     - :ref:`Quadratic - MIQCP Method <option-GUROBI-miqcp_method>`
   * - MIRCUTS
     - :ref:`MIP Cuts - MIR Cuts <option-GUROBI-mir_cuts>`
   * - MIXINGCUTS
     - :ref:`MIP Cuts - Mixing Cuts <option-GUROBI-mixing_cuts>`
   * - MODKCUTS
     - :ref:`MIP Cuts - Mod K Cuts <option-GUROBI-mod_k_cuts>`
   * - MULTIOBJMETHOD
     - :ref:`General - Multi-objective Method <option-GUROBI-multi_objective_method>`
   * - MULTIOBJPRE
     - :ref:`Presolve - Multi-objective Presolve <option-GUROBI-multi_objective_presolve>`
   * - NETWORKALG
     - :ref:`Simplex - Network Algorithm <option-GUROBI-network_algorithm>`
   * - NETWORKCUTS
     - :ref:`MIP Cuts - Network Cuts <option-GUROBI-network_cuts>`
   * - NLPHEUR
     - :ref:`Nonlinear - NLP Heuristic <option-GUROBI-nlp_heuristic>`
   * - NODEFILESTART
     - :ref:`MIP - Node File Start <option-GUROBI-node_file_start>`
   * - NODELIMIT
     - :ref:`MIP - Node Limit <option-GUROBI-node_limit>`
   * - NODEMETHOD
     - :ref:`MIP - MIP Node Method <option-GUROBI-mip_node_method>`
   * - NONCONVEX
     - :ref:`Quadratic - Nonconvex Strategy <option-GUROBI-nonconvex_strategy>`
   * - NORELHEURSOLUTIONS
     - :ref:`MIP Heuristics - No Relaxation Heuristic Limit <option-GUROBI-no_relaxation_heuristic_limit>`
   * - NORELHEURTIME
     - :ref:`MIP Heuristics - No Relaxation Heuristic Time <option-GUROBI-no_relaxation_heuristic_time>`
   * - NORELHEURWORK
     - :ref:`MIP Heuristics - No Relaxation Heuristic Work <option-GUROBI-no_relaxation_heuristic_work>`
   * - NORMADJUST
     - :ref:`Simplex - Norm Adjust <option-GUROBI-norm_adjust>`
   * - NUMERICFOCUS
     - :ref:`General - Numeric Focus <option-GUROBI-numeric_focus>`
   * - OBBT
     - :ref:`MIP Presolve - MIP OBBT <option-GUROBI-mip_obbt>`
   * - OBJSCALE
     - :ref:`Simplex - Objective Scale <option-GUROBI-objective_scale>`
   * - OPTIMALITYTOL
     - :ref:`General - Optimality Tolerance <option-GUROBI-optimality>`
   * - OUTPUTFLAG
     - :ref:`Logging - Output File <option-GUROBI-output_file>`
   * - PARTITIONPLACE
     - :ref:`MIP Heuristics - Partition Heuristic <option-GUROBI-partition_heuristic>`
   * - PDHGABSTOL
     - :ref:`PDHG - PDHG Absolute Feasibility Tolerance <option-GUROBI-pdhg_absolute_feasibility_tolerance>`
   * - PDHGCONVTOL
     - :ref:`PDHG - PDHG Convergence Tolerance <option-GUROBI-pdhg_convergence_tolerance>`
   * - PDHGITERLIMIT
     - :ref:`PDHG - PDHG Iteration Limit <option-GUROBI-pdhg_iteration_limit>`
   * - PDHGRELTOL
     - :ref:`PDHG - PDHG Relative Feasibility Tolerance <option-GUROBI-pdhg_relative_feasibility_tolerance>`
   * - PERTURBVALUE
     - :ref:`Simplex - Perturbation <option-GUROBI-perturbation>`
   * - POOLGAP
     - :ref:`Solution Pool - Pool Gap <option-GUROBI-pool_gap>`
   * - POOLGAPABS
     - :ref:`Solution Pool - Pool Absolute Gap <option-GUROBI-pool_absolute_gap>`
   * - POOLSEARCHMODE
     - :ref:`Solution Pool - Pool Search Mode <option-GUROBI-pool_search_mode>`
   * - POOLSOLUTIONS
     - :ref:`Solution Pool - Pool Size <option-GUROBI-pool_size>`
   * - PREDEPROW
     - :ref:`Presolve - Presolve Row Reduction <option-GUROBI-presolve_row_reduction>`
   * - PREDUAL
     - :ref:`Presolve - Presolve Dual <option-GUROBI-presolve_dual>`
   * - PREMIQCPFORM
     - :ref:`Quadratic - MIQCP Formulation <option-GUROBI-miqcp_formulation>`
   * - PREPASSES
     - :ref:`PPresolve - resolve Passes <option-GUROBI-presolve_passes>`
   * - PREQLINEARIZE
     - :ref:`Presolve - Linearize Quadratic Constraints <option-GUROBI-linearize_quadratic_constraints>`
   * - PRESOLVE
     - :ref:`Presolve - Presolve <option-GUROBI-presolve>`
   * - PRESOS1BIGM
     - :ref:`MIP Presolve - SOS1 Reformulation Threshold <option-GUROBI-sos1_reformulation_threshold>`
   * - PRESOS1ENCODING
     - :ref:`MIP Presolve - SOS1 Encoding <option-GUROBI-sos1_encoding>`
   * - PRESOS2BIGM
     - :ref:`MIP Presolve - SOS2 Reformulation Threshold <option-GUROBI-sos2_reformulation_threshold>`
   * - PRESOS2ENCODING
     - :ref:`MIP Presolve - SOS2 Encoding <option-GUROBI-sos2_encoding>`
   * - PRESPARSIFY
     - :ref:`MIP Presolve - Presolve Sparsify Reduction <option-GUROBI-presolve_sparsify_reduction>`
   * - PROJIMPLIEDCUTS
     - :ref:`MIP Cuts - Projected Implied Bound Cuts <option-GUROBI-projected_implied_bound_cuts>`
   * - PSDTOL
     - :ref:`Quadratic - PSD Tolerance <option-GUROBI-psd_tolerance>`
   * - PUMPPASSES
     - :ref:`MIP Heuristics - Feasibility Pump Passes <option-GUROBI-feasibility_pump_passes>`
   * - QCPDUAL
     - :ref:`Quadratic - QCP Dual Values <option-GUROBI-qcp_dual_values>`
   * - QUAD
     - :ref:`Simplex - Quad Precision <option-GUROBI-quad_precision>`
   * - RELAXLIFTCUTS
     - :ref:`MIP Cuts - Relax-and-Lift Cuts <option-GUROBI-relax-and-lift_cuts>`
   * - RINS
     - :ref:`MIP Heuristics - RINS Heuristic Frequency <option-GUROBI-rins_heuristic_frequency>`
   * - RLTCUTS
     - :ref:`MIP Cuts - RLT Cuts <option-GUROBI-rlt_cuts>`
   * - SCALEFLAG
     - :ref:`General - Scale <option-GUROBI-scale>`
   * - SEED
     - :ref:`General - Random Seed <option-GUROBI-random_seed>`
   * - SIFTING
     - :ref:`Simplex - Sifting <option-GUROBI-sifting>`
   * - SIFTMETHOD
     - :ref:`Simplex - Sifting Method <option-GUROBI-sifting_method>`
   * - SIMPLEXPRICING
     - :ref:`Simplex - Pricing <option-GUROBI-pricing>`
   * - SOFTMEMLIMIT
     - :ref:`General - Soft Memory Limit <option-GUROBI-soft_memory_limit>`
   * - SOLUTIONTARGET
     - :ref:`General - Solution Target <option-GUROBI-solution_target>`
   * - STARTNODELIMIT
     - :ref:`MIP - MIP Start Node Limit <option-GUROBI-mip_start_node_limit>`
   * - STARTTIMELIMIT
     - :ref:`MIP - MIP Start Time Limit <option-GUROBI-mip_start_time_limit>`
   * - STARTWORKLIMIT
     - :ref:`MIP - MIP Start Work Limit <option-GUROBI-mip_start_work_limit>`
   * - STRONGCGCUTS
     - :ref:`MIP Cuts - Strong CG Cuts <option-GUROBI-strong_cg_cuts>`
   * - SUBMIPCUTS
     - :ref:`MIP Cuts - Sub MIP Cuts <option-GUROBI-sub_mip_cuts>`
   * - SUBMIPNODES
     - :ref:`MIP Heuristics - RINS Sub-MIP Node Limit <option-GUROBI-rins_sub_mip_node_limit>`
   * - SYMMETRY
     - :ref:`MIP - MIP Symmetry <option-GUROBI-mip_symmetry>`
   * - THREADS
     - :ref:`Parallel - Thread Limit <option-GUROBI-thread_limit>`
   * - TUNECLEANUP
     - :ref:`Tuning - Tune Cleanup <option-GUROBI-tune_cleanup>`
   * - TUNECRITERION
     - :ref:`Tuning - Tune Criterion <option-GUROBI-tune_criterion>`
   * - TUNEMETRIC
     - :ref:`Tuning - Tune Metric <option-GUROBI-tune_metric>`
   * - TUNEOUTPUT
     - :ref:`Logging - Tune Output Level <option-GUROBI-tune_output_level>`
   * - TUNERESULTS
     - :ref:`Tuning - Tune Results <option-GUROBI-tune_results>`
   * - TUNETARGETMIPGAP
     - :ref:`Tuning - Tune Target MIP Gap <option-GUROBI-tune_target_mip_gap>`
   * - TUNETARGETTIME
     - :ref:`Tuning - Tune Target Time <option-GUROBI-tune_target_time>`
   * - TUNETIMELIMIT
     - :ref:`Tuning - Tune Time Limit <option-GUROBI-tune_time_limit>`
   * - TUNETRIALS
     - :ref:`Tuning - Tune Trials <option-GUROBI-tune_trials>`
   * - VARBRANCH
     - :ref:`MIP - Select Variables <option-GUROBI-select_variables>`
   * - WORKLIMIT
     - :ref:`General - Work Limit <option-GUROBI-work_limit>`
   * - ZEROHALFCUTS
     - :ref:`MIP Cuts - Zero Half Cuts <option-GUROBI-zero_half_cuts>`
   * - ZEROOBJNODES
     - :ref:`MIP Heuristics - Zero Objective Node Limit <option-GUROBI-zero_objective_node_limit>`


**Note** 

*	The Gurobi parameter PRECRUSH is not available in AIMMS. AIMMS automatically switches it on when a cut callback procedure is installed in the AIMMS model.
