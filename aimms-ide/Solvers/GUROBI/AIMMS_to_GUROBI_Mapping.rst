

.. _AIMMS_to_GUROBI_Mapping:


AIMMS to Gurobi Mapping
============================

**Description** 

The table shows in the left column the AIMMS Gurobi options while the right column displays the associated Gurobi parameter.

.. list-table::

   * - **Option name in AIMMS** 
     - **Name in Gurobi** 
   * - :ref:`Barrier - Barrier Convergence Tolerance <option-GUROBI-barrier_convergence_tolerance>`
     - BARCONVTOL
   * - :ref:`Barrier - Barrier Correction Steps <option-GUROBI-barrier_correction_steps>`
     - BARCORRECTORS
   * - :ref:`Barrier - Barrier Crossover <option-GUROBI-barrier_crossover>`
     - CROSSOVER
   * - :ref:`Barrier - Barrier Crossover Basis <option-GUROBI-barrier_crossover_basis>`
     - CROSSOVERBASIS
   * - :ref:`Barrier - Barrier Homogeneous Algorithm <option-GUROBI-barrier_homogeneous_algorithm>`
     - BARHOMOGENEOUS
   * - :ref:`Barrier - Barrier Iteration Limit <option-GUROBI-barrier_iteration_limit>`
     - BARITERLIMIT
   * - :ref:`Barrier - Barrier Ordering <option-GUROBI-barrier_ordering>`
     - BARORDER
   * - :ref:`Barrier - Barrier Progress Solution <option-GUROBI-barrier_progress_solution>`
     - 
   * - :ref:`Barrier - Barrier QCP Convergence Tolerance <option-GUROBI-barrier_qcp_convergence_tolerance>`
     - BARQCPCONVTOL
   * - :ref:`General - Calculate Kappa <option-GUROBI-calculate_kappa>`
     - 
   * - :ref:`General - Concurrent Method <option-GUROBI-concurrent_method>`
     - CONCURRENTMETHOD
   * - :ref:`General - Farkas Infeasibility Proof <option-GUROBI-farkas_infeasibility_proof>`
     - 
   * - :ref:`General - Feasibility Tolerance <option-GUROBI-feasibility>`
     - FEASIBILITYTOL
   * - :ref:`General - IIS Method <option-GUROBI-iis_method>`
     - FEASRELAXBIGM
   * - :ref:`General - IIS Method <option-GUROBI-iis_method>`
     - IISMETHOD
   * - :ref:`General - Memory Limit <option-GUROBI-memory_limit>`
     - MEMLIMIT
   * - :ref:`General - Method <option-GUROBI-method>`
     - METHOD
   * - :ref:`General - MPS <option-GUROBI-mps>`
     - 
   * - :ref:`General - MPS Dual <option-GUROBI-mps_dual>`
     - 
   * - :ref:`General - Multi-objective Method <option-GUROBI-multi_objective_method>`
     - MULTIOBJMETHOD
   * - :ref:`General - Numeric Focus <option-GUROBI-numeric_focus>`
     - NUMERICFOCUS
   * - :ref:`General - Optimality Tolerance <option-GUROBI-optimality>`
     - OPTIMALITYTOL
   * - :ref:`General - Random Seed <option-GUROBI-random_seed>`
     - SEED
   * - :ref:`General - Read Parameter File <option-GUROBI-read_parameter_file>`
     - 
   * - :ref:`General - Restart <option-GUROBI-restart>`
     - 
   * - :ref:`General - Restart File Number <option-GUROBI-restart_file_number>`
     - 
   * - :ref:`General - Scale <option-GUROBI-scale>`
     - SCALEFLAG
   * - :ref:`General - Sensitivity Method <option-GUROBI-sensitivity_method>`
     - 
   * - :ref:`General - Soft Memory Limit <option-GUROBI-soft_memory_limit>`
     - SOFTMEMLIMIT
   * - :ref:`General - Solution File <option-GUROBI-solution_file>`
     - 
   * - :ref:`General - Solution Target <option-GUROBI-solution_target>`
     - SOLUTIONTARGET
   * - :ref:`General - Unbounded Ray <option-GUROBI-unbounded_ray>`
     - 
   * - :ref:`General - Updates Batch Size <option-GUROBI-updates_batch_size>`
     - 
   * - :ref:`General - Warm Start <option-GUROBI-warm_start>`
     - LPWARMSTART
   * - :ref:`General - Work Limit <option-GUROBI-work_limit>`
     - WORKLIMIT
   * - :ref:`General - Write Parameter File <option-GUROBI-write_parameter_file>`
     - 
   * - :ref:`Logging - Display Solution Quality <option-GUROBI-display_solution_quality>`
     - 
   * - :ref:`Logging - Log to Console <option-GUROBI-log_to_console>`
     - LOGTOCONSOLE
   * - :ref:`Logging - Output File <option-GUROBI-output_file>`
     - OUTPUTFLAG
   * - :ref:`Logging - Output File Display Interval <option-GUROBI-output_file_display_interval>`
     - DISPLAYINTERVAL
   * - :ref:`Logging - Tune Output Level <option-GUROBI-tune_output_level>`
     - TUNEOUTPUT
   * - :ref:`MIP - Branch Direction <option-GUROBI-branch_direction>`
     - BRANCHDIR
   * - :ref:`MIP - Disconnected Component Strategy <option-GUROBI-disconnected_component_strategy>`
     - DISCONNECTED
   * - :ref:`MIP - Hints File <option-GUROBI-hints_file>`
     - 
   * - :ref:`MIP - Improve Start Gap <option-GUROBI-improve_start_gap>`
     - IMPROVESTARTGAP
   * - :ref:`MIP - Improve Start Nodes <option-GUROBI-improve_start_nodes>`
     - IMPROVESTARTNODES
   * - :ref:`MIP - Improve Start Time <option-GUROBI-improve_start_time>`
     - IMPROVESTARTTIME
   * - :ref:`MIP - Improve Start Work <option-GUROBI-improve_start_work>`
     - IMPROVESTARTWORK
   * - :ref:`MIP - Integrality Tolerance <option-GUROBI-integrality>`
     - INTFEASTOL
   * - :ref:`MIP - Integrality Focus <option-GUROBI-integrality_focus>`
     - INTEGRALITYFOCUS
   * - :ref:`MIP - Lazy Constraint Mode <option-GUROBI-lazy_constraint_mode>`
     - 
   * - :ref:`MIP - MIP Best Bound Stop <option-GUROBI-mip_best_bound_stop>`
     - BESTBDSTOP
   * - :ref:`MIP - MIP Best Objective Stop <option-GUROBI-mip_best_objective_stop>`
     - BESTOBJSTOP
   * - :ref:`MIP - MIP Focus <option-GUROBI-mip_focus>`
     - MIPFOCUS
   * - :ref:`MIP - MIP Node Method <option-GUROBI-mip_node_method>`
     - NODEMETHOD
   * - :ref:`MIP - MIP Start <option-GUROBI-mip_start>`
     - 
   * - :ref:`MIP - MIP Start Node Limit <option-GUROBI-mip_start_node_limit>`
     - STARTNODELIMIT
   * - :ref:`MIP - MIP Start Time Limit <option-GUROBI-mip_start_time_limit>`
     - STARTTIMELIMIT
   * - :ref:`MIP - MIP Start Work Limit <option-GUROBI-mip_start_work_limit>`
     - STARTWORKLIMIT
   * - :ref:`MIP - MIP Symmetry <option-GUROBI-mip_symmetry>`
     - SYMMETRY
   * - :ref:`MIP - Node File Start <option-GUROBI-node_file_start>`
     - NODEFILESTART
   * - :ref:`MIP - Node Limit <option-GUROBI-node_limit>`
     - NODELIMIT
   * - :ref:`MIP - Select Variables <option-GUROBI-select_variables>`
     - VARBRANCH
   * - :ref:`MIP Cuts - BQP Cuts <option-GUROBI-bqp_cuts>`
     - BQPCUTS
   * - :ref:`MIP Cuts - Clique Cuts <option-GUROBI-clique_cuts>`
     - CLIQUECUTS
   * - :ref:`MIP Cuts - Cover Cuts <option-GUROBI-cover_cuts>`
     - COVERCUTS
   * - :ref:`MIP Cuts - Dual Implied Cuts <option-GUROBI-dual_implied_cuts>`
     - DUALIMPLIEDCUTS
   * - :ref:`MIP Cuts - Cut Aggregation Passes Limit <option-GUROBI-cut_aggregation_passes_limit>`
     - CUTAGGPASSES
   * - :ref:`MIP Cuts - Flow Cover Cuts <option-GUROBI-flow_cover_cuts>`
     - FLOWCOVERCUTS
   * - :ref:`MIP Cuts - Flow Path Cuts <option-GUROBI-flow_path_cuts>`
     - FLOWPATHCUTS
   * - :ref:`MIP Cuts - Global Cut Control <option-GUROBI-global_cut_control>`
     - CUTS
   * - :ref:`MIP Cuts - Gomory Cut Passes Limit <option-GUROBI-gomory_cut_passes_limit>`
     - GOMORYPASSES
   * - :ref:`MIP Cuts - GUB Cover Cuts <option-GUROBI-gub_cover_cuts>`
     - GUBCOVERCUTS
   * - :ref:`MIP Cuts - Implied Bound Cuts <option-GUROBI-implied_bound_cuts>`
     - IMPLIEDCUTS
   * - :ref:`MIP Cuts - Infeasibility Proof Cuts <option-GUROBI-infeasibility_proof_cuts>`
     - INFPROOFCUTS
   * - :ref:`MIP Cuts - Lift and Project Cuts <option-GUROBI-lift_and_project_cuts>`
     - LIFTPROJECTCUTS
   * - :ref:`MIP Cuts - Master Knapsack Cuts <option-GUROBI-master_knapsack_cuts>`
     - MASTERKNAPSACKCUTS
   * - :ref:`MIP Cuts - MIP Separation Cuts <option-GUROBI-mip_separation_cuts>`
     - MIPSEPCUTS
   * - :ref:`MIP Cuts - MIR Cuts <option-GUROBI-mir_cuts>`
     - MIRCUTS
   * - :ref:`MIP Cuts - Mixing Cuts <option-GUROBI-mixing_cuts>`
     - MIXINGCUTS
   * - :ref:`MIP Cuts - Mod K Cuts <option-GUROBI-mod_k_cuts>`
     - MODKCUTS
   * - :ref:`MIP Cuts - Network Cuts <option-GUROBI-network_cuts>`
     - NETWORKCUTS
   * - :ref:`MIP Cuts - Projected Implied Bound Cuts <option-GUROBI-projected_implied_bound_cuts>`
     - PROJIMPLIEDCUTS
   * - :ref:`MIP Cuts - Relax-and-Lift Cuts <option-GUROBI-relax-and-lift_cuts>`
     - RELAXLIFTCUTS
   * - :ref:`MIP Cuts - RLT Cuts <option-GUROBI-rlt_cuts>`
     - RLTCUTS
   * - :ref:`MIP Cuts - Root Cut Passes Limit <option-GUROBI-root_cut_passes_limit>`
     - CUTPASSES
   * - :ref:`MIP Cuts - Strong CG Cuts <option-GUROBI-strong_cg_cuts>`
     - STRONGCGCUTS
   * - :ref:`MIP Cuts - Sub MIP Cuts <option-GUROBI-sub_mip_cuts>`
     - SUBMIPCUTS
   * - :ref:`MIP Cuts - Zero Half Cuts <option-GUROBI-zero_half_cuts>`
     - ZEROHALFCUTS
   * - :ref:`MIP Heuristics - Feasibility Pump Passes <option-GUROBI-feasibility_pump_passes>`
     - PUMPPASSES
   * - :ref:`MIP Heuristics - Heuristics <option-GUROBI-heuristics>`
     - HEURISTICS
   * - :ref:`MIP Heuristics - Minimum Relaxation Heuristic Node Limit <option-GUROBI-minimum_relaxation_heuristic_node_limit>`
     - MINRELNODES
   * - :ref:`MIP Heuristics - No Relaxation Heuristic Limit <option-GUROBI-no_relaxation_heuristic_limit>`
     - NORELHEURSOLUTIONS
   * - :ref:`MIP Heuristics - No Relaxation Heuristic Time <option-GUROBI-no_relaxation_heuristic_time>`
     - NORELHEURTIME
   * - :ref:`MIP Heuristics - No Relaxation Heuristic Work <option-GUROBI-no_relaxation_heuristic_work>`
     - NORELHEURWORK
   * - :ref:`MIP Heuristics - Partition Heuristic <option-GUROBI-partition_heuristic>`
     - PARTITIONPLACE
   * - :ref:`MIP Heuristics - RINS Heuristic Frequency <option-GUROBI-rins_heuristic_frequency>`
     - RINS
   * - :ref:`MIP Heuristics - RINS Sub-MIP Node Limit <option-GUROBI-rins_sub_mip_node_limit>`
     - SUBMIPNODES
   * - :ref:`MIP Heuristics - Zero Objective Node Limit <option-GUROBI-zero_objective_node_limit>`
     - ZEROOBJNODES
   * - :ref:`MIP Presolve - MIP OBBT <option-GUROBI-mip_obbt>`
     - OBBT
   * - :ref:`MIP Presolve - Presolve Sparsify Reduction <option-GUROBI-presolve_sparsify_reduction>`
     - PRESPARSIFY
   * - :ref:`MIP Presolve - SOS1 Encoding <option-GUROBI-sos1_encoding>`
     - PRESOS1ENCODING
   * - :ref:`MIP Presolve - SOS1 Reformulation Threshold <option-GUROBI-sos1_reformulation_threshold>`
     - PRESOS1BIGM
   * - :ref:`MIP Presolve - SOS2 Encoding <option-GUROBI-sos2_encoding>`
     - PRESOS2ENCODING
   * - :ref:`MIP Presolve - SOS2 Reformulation Threshold <option-GUROBI-sos2_reformulation_threshold>`
     - PRESOS2BIGM
   * - :ref:`Nonlinear - Maximal Variable Bound <option-GUROBI-maximal_variable_bound>`
     - 
   * - :ref:`Nonlinear - NLP Heuristic <option-GUROBI-nlp_heuristic>`
     - NLPHEUR
   * - :ref:`Nonlinear - Nonlinear Optimality Tolerance <option-GUROBI-nonlinear_optimality_tolerance>`
     - MIPGAP
   * - :ref:`Parallel - Concurrent MIP <option-GUROBI-concurrent_mip>`
     - CONCURRENTMIP
   * - :ref:`Parallel - Thread Limit <option-GUROBI-thread_limit>`
     - THREADS
   * - :ref:`PDHG - PDHG Absolute Feasibility Tolerance <option-GUROBI-pdhg_absolute_feasibility_tolerance>`
     - PDHGABSTOL
   * - :ref:`PDHG - PDHG Convergence Tolerance <option-GUROBI-pdhg_convergence_tolerance>`
     - PDHGCONVTOL
   * - :ref:`PDHG - PDHG Iteration Limit <option-GUROBI-pdhg_iteration_limit>`
     - PDHGITERLIMIT
   * - :ref:`PDHG - PDHG Relative Feasibility Tolerance <option-GUROBI-pdhg_relative_feasibility_tolerance>`
     - PDHGRELTOL
   * - :ref:`Presolve - Dual Reductions <option-GUROBI-dual_reductions>`
     - DUALREDUCTIONS
   * - :ref:`Presolve - Linearize Quadratic Constraints <option-GUROBI-linearize_quadratic_constraints>`
     - PREQLINEARIZE
   * - :ref:`Presolve - Multi-objective Presolve <option-GUROBI-multi_objective_presolve>`
     - MULTIOBJPRE
   * - :ref:`Presolve - Presolve <option-GUROBI-presolve>`
     - PRESOLVE
   * - :ref:`Presolve - Presolve Aggregation <option-GUROBI-presolve_aggregation>`
     - AGGREGATE
   * - :ref:`Presolve - Presolve Aggregation Fill <option-GUROBI-presolve_aggregation_fill>`
     - AGGFILL
   * - :ref:`Presolve - Presolve Dual <option-GUROBI-presolve_dual>`
     - PREDUAL
   * - :ref:`PPresolve - resolve Passes <option-GUROBI-presolve_passes>`
     - PREPASSES
   * - :ref:`Presolve - Presolve Row Reduction <option-GUROBI-presolve_row_reduction>`
     - PREDEPROW
   * - :ref:`Quadratic - MIQCP Formulation <option-GUROBI-miqcp_formulation>`
     - PREMIQCPFORM
   * - :ref:`Quadratic - MIQCP Method <option-GUROBI-miqcp_method>`
     - MIQCPMETHOD
   * - :ref:`Quadratic - Nonconvex Strategy <option-GUROBI-nonconvex_strategy>`
     - NONCONVEX
   * - :ref:`Quadratic - PSD Tolerance <option-GUROBI-psd_tolerance>`
     - PSDTOL
   * - :ref:`Quadratic - QCP Dual Values <option-GUROBI-qcp_dual_values>`
     - QCPDUAL
   * - :ref:`Simplex - Degenerate Simplex Moves Limit <option-GUROBI-degenerate_simplex_moves_limit>`
     - DEGENMOVES
   * - :ref:`Simplex - Markowitz Tolerance <option-GUROBI-markowitz>`
     - MARKOWITZTOL
   * - :ref:`Simplex - Network Algorithm <option-GUROBI-network_algorithm>`
     - NETWORKALG
   * - :ref:`Simplex - Norm Adjust <option-GUROBI-norm_adjust>`
     - NORMADJUST
   * - :ref:`Simplex - Objective Scale <option-GUROBI-objective_scale>`
     - OBJSCALE
   * - :ref:`Simplex - Perturbation <option-GUROBI-perturbation>`
     - PERTURBVALUE
   * - :ref:`Simplex - Pricing <option-GUROBI-pricing>`
     - SIMPLEXPRICING
   * - :ref:`Simplex - Quad Precision <option-GUROBI-quad_precision>`
     - QUAD
   * - :ref:`Simplex - Sifting <option-GUROBI-sifting>`
     - SIFTING
   * - :ref:`Simplex - Sifting Method <option-GUROBI-sifting_method>`
     - SIFTMETHOD
   * - :ref:`Solution Pool - Pool Absolute Gap <option-GUROBI-pool_absolute_gap>`
     - POOLGAPABS
   * - :ref:`Solution Pool - Pool Gap <option-GUROBI-pool_gap>`
     - POOLGAP
   * - :ref:`Solution Pool - Pool Search Mode <option-GUROBI-pool_search_mode>`
     - POOLSEARCHMODE
   * - :ref:`Solution Pool - Pool Size <option-GUROBI-pool_size>`
     - POOLSOLUTIONS
   * - :ref:`Tuning - Tune Cleanup <option-GUROBI-tune_cleanup>`
     - TUNECLEANUP
   * - :ref:`Tuning - Tune Criterion <option-GUROBI-tune_criterion>`
     - TUNECRITERION
   * - :ref:`Tuning - Tune Metric <option-GUROBI-tune_metric>`
     - TUNEMETRIC
   * - :ref:`Tuning - Tune Results <option-GUROBI-tune_results>`
     - TUNERESULTS
   * - :ref:`Tuning - Tune Target MIP Gap <option-GUROBI-tune_target_mip_gap>`
     - TUNETARGETMIPGAP
   * - :ref:`Tuning - Tune Target Time <option-GUROBI-tune_target_time>`
     - TUNETARGETTIME
   * - :ref:`Tuning - Tune Time Limit <option-GUROBI-tune_time_limit>`
     - TUNETIMELIMIT
   * - :ref:`Tuning - Tune Trials <option-GUROBI-tune_trials>`
     - TUNETRIALS


The table below shows Solvers General options that are mapped to Gurobi parameters.

.. list-table::

   * - **Option name in AIMMS** 
     - **Name in GUROBI** 
   * - :ref:`MIP Options - Cutoff <option-AIMMS-cutoff>`
     - CUTOFF
   * - :ref:`MIP Options - Maximal Number of Integer Solutions <option-AIMMS-maximal_number_of_integer_solutions>`
     - SOLUTIONLIMIT
   * - :ref:`MIP Options - MIP Absolute Optimality Tolerance <option-AIMMS-mip_absolute_optimality_tolerance>`
     - MIPGAPABS
   * - :ref:`MIP Options - MIP Relative Optimality Tolerance <option-AIMMS-mip_relative_optimality_tolerance>`
     - MIPGAP
   * - :ref:`Stop Criteria - Iteration Limit <option-AIMMS-iteration_limit>`
     - ITERATIONLIMIT
   * - :ref:`Stop Criteria - Time Limit <option-AIMMS-time_limit>`
     - TIMELIMIT



