

.. _CPLEX_to_AIMMS_Mapping:


CPLEX to AIMMS Mapping
===========================

**Description** 

The table shows in the left column the parameters from CPLEX that can be set in AIMMS; the right column displays for each CPLEX parameter the associated AIMMS option.

.. list-table::
   :header-rows: 0

   * - **Name in CPLEX**
     - **Option name in AIMMS** 
   * - Advance
     - :ref:`General - Advanced Start <option-CPLEX-advanced_start>`
   * - Bar qcpconvergetol
     - :ref:`QP - Barrier Convergence Tolerance for QCP <option-CPLEX-barrier_convergence_tolerance_for_qcp>`
   * - Barrier algorithm
     - :ref:`Barrier - Barrier Algorithm <option-CPLEX-barrier_algorithm>`
   * - Barrier colnonzeros
     - :ref:`Barrier - Barrier Density Definition <option-CPLEX-barrier_density_definition>`
   * - Barrier convergetol
     - :ref:`Barrier - Barrier Convergence Tolerance <option-CPLEX-barrier_convergence_tolerance>`
   * - Barrier crossover
     - :ref:`Barrier - Barrier Crossover Algorithm <option-CPLEX-barrier_crossover_algorithm>`
   * - Barrier display
     - :ref:`Logging - Barrier Display <option-CPLEX-barrier_display>`
   * - Barrier limits corrections
     - :ref:`Barrier - Barrier Maximal Number of Corrections <option-CPLEX-barrier_maximal_number_of_corrections>`
   * - Barrier limits growth
     - :ref:`Barrier - Barrier Growth Limit <option-CPLEX-barrier_growth_limit>`
   * - Barrier limits iteration
     - :ref:`Barrier - Barrier Iterations <option-CPLEX-barrier_iterations>`
   * - Barrier limits objrange
     - :ref:`Barrier - Barrier Objective Range <option-CPLEX-barrier_objective_range>`
   * - Barrier ordering
     - :ref:`Barrier - Barrier Ordering <option-CPLEX-barrier_ordering>`
   * - Barrier startalg
     - :ref:`Barrier - Barrier Start Algorithm <option-CPLEX-barrier_start_algorithm>`
   * - Benders strategy
     - :ref:`Benders - Benders Strategy <option-CPLEX-benders_strategy>`
   * - Benders tolerances feasibilitycut
     - :ref:`Benders - Benders Feasibility Cut Tolerance <option-CPLEX-benders_feasibility_cut_tolerance>`
   * - Benders tolerances optimalitycut
     - :ref:`Benders - Benders Optimality Cut Tolerance <option-CPLEX-benders_optimality_cut_tolerance>`
   * - Benders workeralgorithm
     - :ref:`Benders - Benders Worker Algorithm <option-CPLEX-benders_worker_algorithm>`
   * - Clocktype
     - :ref:`General - Clock Type <option-CPLEX-clock_type>`
   * - Conflict algorithm
     - :ref:`General - Conflict Algorithm <option-CPLEX-conflict_algorithm>`
   * - Dettimelimit
     - :ref:`General - Deterministic Time Limit <option-CPLEX-deterministic_time_limit>`
   * - Emphasis memory
     - :ref:`General - Memory Emphasis <option-CPLEX-memory_emphasis>`
   * - Emphasis MIP
     - :ref:`MIP - MIP Emphasis <option-CPLEX-mip_emphasis>`
   * - Emphasis numerical
     - :ref:`General - Numerical Emphasis <option-CPLEX-numerical_emphasis>`
   * - Feasopt tolerance
     - :ref:`General - Feasopt Tolerance <option-CPLEX-feasopt_tolerance>`
   * - Lpmethod
     - :ref:`General - LP Method <option-CPLEX-lp_method>`
   * - MIP cuts bqp
     - :ref:`MIP Cuts - Bqp Cuts <option-CPLEX-bqp_cuts>`
   * - MIP cuts cliques
     - :ref:`MIP Cuts - Clique Cuts <option-CPLEX-clique_cuts>`
   * - MIP cuts covers
     - :ref:`MIP Cuts - Cover Cuts <option-CPLEX-cover_cuts>`
   * - MIP cuts disjunctive
     - :ref:`MIP Cuts - Disjunctive Cuts <option-CPLEX-disjunctive_cuts>`
   * - MIP cuts flow
     - :ref:`MIP Cuts - Flow Cover Cuts <option-CPLEX-flow_cover_cuts>`
   * - MIP cuts gomory
     - :ref:`MIP Cuts - Gomory Cuts <option-CPLEX-gomory_cuts>`
   * - MIP cuts gubcovers
     - :ref:`MIP Cuts - Gub Cover Cuts <option-CPLEX-gub_cover_cuts>`
   * - MIP cuts implied
     - :ref:`MIP Cuts - Implied Bound Cuts <option-CPLEX-implied_bound_cuts>`
   * - MIP cuts liftproj
     - :ref:`MIP Cuts - Lift and Project Cuts <option-CPLEX-lift_and_project_cuts>`
   * - MIP cuts localimplied
     - :ref:`MIP Cuts - Local Implied Bound Cuts <option-CPLEX-local_implied_bound_cuts>`
   * - MIP cuts mcfcut
     - :ref:`MIP Cuts - MCF Cuts <option-CPLEX-mcf_cuts>`
   * - MIP cuts mircut
     - :ref:`MIP Cuts - Mixed Integer Rounding Cuts <option-CPLEX-mixed_integer_rounding_cuts>`
   * - MIP cuts nodecuts
     - :ref:`MIP Cuts - Node Cuts <option-CPLEX-node_cuts>`
   * - MIP cuts pathcut
     - :ref:`MIP Cuts - Flow Path Cuts <option-CPLEX-flow_path_cuts>`
   * - MIP cuts rlt
     - :ref:`MIP Cuts - RLT Cuts <option-CPLEX-rlt_cuts>`
   * - MIP cuts zerohalf
     - :ref:`MIP Cuts - Zero Half Cuts <option-CPLEX-zero_half_cuts>`
   * - MIP display
     - :ref:`Logging - MIP Display <option-CPLEX-mip_display>`
   * - MIP interval
     - :ref:`Logging - MIP Interval <option-CPLEX-mip_interval>`
   * - MIP limits aggforcut
     - :ref:`MIP Cuts - Cut Generation Limit <option-CPLEX-cut_generation_limit>`
   * - MIP limits auxrootthreads
     - :ref:`Parallel - Auxiliary Root Threads <option-CPLEX-auxiliary_root_threads>`
   * - MIP limits cutpasses
     - :ref:`MIP Cuts - MIP Number of Cut Passes <option-CPLEX-mip_number_of_cut_passes>`
   * - MIP limits cutsfactor
     - :ref:`MIP Cuts - Cuts Factor <option-CPLEX-cuts_factor>`
   * - MIP limits eachcutlimit
     - :ref:`MIP Cuts - Cut Limit <option-CPLEX-cut_limit>`
   * - MIP limits gomorycand
     - :ref:`MIP Cuts - Gomory Cuts Candidate Limit <option-CPLEX-gomory_cuts_candidate_limit>`
   * - MIP limits gomorypass
     - :ref:`MIP Cuts - Gomory Cuts Pass Limit <option-CPLEX-gomory_cuts_pass_limit>`
   * - MIP limits lowerobjstop
     - :ref:`MIP Advanced - Lower Objective Stop <option-CPLEX-lower_objective_stop>`
   * - MIP limits nodes
     - :ref:`MIP - Maximal Number of Nodes <option-CPLEX-maximal_number_of_nodes>`
   * - MIP limits populate
     - :ref:`MIP Solution Pool - Population Limit <option-CPLEX-population_limit>`
   * - MIP limits probedettime
     - :ref:`MIP - Probing Time Deterministic <option-CPLEX-probing_time_deterministic>`
   * - MIP limits probetime
     - :ref:`MIP - Probing Time <option-CPLEX-probing_time>`
   * - MIP limits repairtries
     - :ref:`MIP - Number of Repair Attempts <option-CPLEX-number_of_repair_attempts>`
   * - MIP limits solutions
     - :ref:`MIP Options - Maximal Number of Integer Solutions <option-AIMMS-maximal_number_of_integer_solutions>`
   * - MIP limits strongcand
     - :ref:`MIP - MIP Candidate List <option-CPLEX-mip_candidate_list>`
   * - MIP limits strongit
     - :ref:`MIP - Number of Simplex Iterations <option-CPLEX-number_of_simplex_iterations>`
   * - MIP limits treememory
     - :ref:`MIP - MIP Tree Memory Limit <option-CPLEX-mip_tree_memory_limit>`
   * - MIP limits upperobjstop
     - :ref:`MIP Advanced - Upper Objective Stop <option-CPLEX-upper_objective_stop>`
   * - MIP ordertype
     - :ref:`MIP - MIP Priority Order Type <option-CPLEX-mip_priority_order_type>`
   * - MIP polishafter absmipgap
     - :ref:`MIP Solution Polishing - Polishing Absolute MIP Gap <option-CPLEX-polishing_absolute_mip_gap>`
   * - MIP polishafter dettime
     - :ref:`MIP Solution Polishing - Polishing Time Deterministic <option-CPLEX-polishing_time_deterministic>`
   * - MIP polishafter mipgap
     - :ref:`MIP Solution Polishing - Polishing Relative MIP Gap <option-CPLEX-polishing_relative_mip_gap>`
   * - MIP polishafter nodes
     - :ref:`MIP Solution Polishing - Polishing Number of Nodes <option-CPLEX-polishing_number_of_nodes>`
   * - MIP polishafter solutions
     - :ref:`MIP Solution Polishing - Polishing Number of Solutions <option-CPLEX-polishing_number_of_solutions>`
   * - MIP polishafter time
     - :ref:`MIP Solution Polishing - Polishing Time <option-CPLEX-polishing_time>`
   * - MIP pool absgap
     - :ref:`MIP Solution Pool - Pool Absolute Objective Gap <option-CPLEX-pool_absolute_objective_gap>`
   * - MIP pool capacity
     - :ref:`MIP Solution Pool - Pool Capacity <option-CPLEX-pool_capacity>`
   * - MIP pool intensity
     - :ref:`MIP Solution Pool - Pool Intensity <option-CPLEX-pool_intensity>`
   * - MIP pool relgap
     - :ref:`MIP Solution Pool - Pool Relative Objective Gap <option-CPLEX-pool_relative_objective_gap>`
   * - MIP pool replace
     - :ref:`MIP Solution Pool - Pool Replacement Strategy <option-CPLEX-pool_replacement_strategy>`
   * - MIP strategy backtrack
     - :ref:`Logging - Backtrack <option-CPLEX-backtrack>`
   * - MIP strategy branch
     - :ref:`MIP - Branch <option-CPLEX-branch>`
   * - MIP strategy dive
     - :ref:`MIP - MIP Dive Strategy <option-CPLEX-mip_dive_strategy>`
   * - MIP strategy file
     - :ref:`MIP - Node File <option-CPLEX-node_file>`
   * - MIP strategy fpheur
     - :ref:`MIP Heuristics - Feasibility Pump Heuristic <option-CPLEX-feasibility_pump_heuristic>`
   * - MIP strategy heuristiceffort
     - :ref:`MIP Heuristics - Heuristic Effort <option-CPLEX-heuristic_effort>`
   * - MIP strategy heuristicfreq
     - :ref:`MIP Heuristics - Heuristic Frequency <option-CPLEX-heuristic_frequency>`
   * - MIP strategy kappastats
     - :ref:`MIP - MIP Kappa <option-CPLEX-mip_kappa>`
   * - MIP strategy lbheur
     - :ref:`MIP Heuristics - Local Branching Heuristic <option-CPLEX-local_branching_heuristic>`
   * - MIP strategy miqcpstrat
     - :ref:`QP - MIQCP Strategy <option-CPLEX-miqcp_strategy>`
   * - MIP strategy nodeselect
     - :ref:`MIP - Selection of Nodes <option-CPLEX-selection_of_nodes>`
   * - MIP strategy order
     - :ref:`MIP - MIP Priority Order Switch <option-CPLEX-mip_priority_order_switch>`
   * - MIP strategy presolvenode
     - :ref:`MIP - MIP Node Presolve <option-CPLEX-mip_node_presolve>`
   * - MIP strategy probe
     - :ref:`MIP - MIP Probing <option-CPLEX-mip_probing>`
   * - MIP strategy rinsheur
     - :ref:`MIP Heuristics - RINS Heuristic Frequency <option-CPLEX-rins_heuristic_frequency>`
   * - MIP strategy search
     - :ref:`MIP - MIP Search Strategy <option-CPLEX-mip_search_strategy>`
   * - MIP strategy startalgorithm
     - :ref:`MIP - MIP Start Algorithm <option-CPLEX-mip_start_algorithm>`
   * - MIP strategy subalgorithm
     - :ref:`MIP - MIP Method <option-CPLEX-mip_method>`
   * - MIP strategy variableselect
     - :ref:`MIP - Select Variables <option-CPLEX-select_variables>`
   * - MIP submip nodelimit
     - :ref:`MIP Advanced - SubMIP Node Limit <option-CPLEX-submip_node_limit>`
   * - MIP submip scale
     - :ref:`MIP Advanced - SubMIP Scale <option-CPLEX-submip_scale>`
   * - MIP submip startalg
     - :ref:`MIP Advanced - SubMIP Start Algorithm <option-CPLEX-submip_start_algorithm>`
   * - MIP submip subalg
     - :ref:`MIP Advanced - SubMIP Subproblem Algorithm <option-CPLEX-submip_subproblem_algorithm>`
   * - MIP tolerances absmipgap
     - :ref:`MIP Options - MIP Absolute Optimality Tolerance <option-AIMMS-mip_absolute_optimality_tolerance>`
   * - MIP tolerances integrality
     - :ref:`MIP - Integrality <option-CPLEX-integrality>`
   * - MIP tolerances lowercutoff
     - :ref:`MIP Options - Cutoff <option-AIMMS-cutoff>`
   * - MIP tolerances mipgap
     - :ref:`MIP Options - MIP Relative Optimality Tolerance <option-AIMMS-mip_relative_optimality_tolerance>`
   * - MIP tolerances objdifference
     - :ref:`MIP - Difference Objective <option-CPLEX-difference_objective>`
   * - MIP tolerances relobjdifference
     - :ref:`MIP - Relative Difference Objective <option-CPLEX-relative_difference_objective>`
   * - MIP tolerances uppercutoff
     - :ref:`MIP Options - Cutoff <option-AIMMS-cutoff>`
   * - Multiobjective display
     - :ref:`Logging - Multi Objective Display <option-CPLEX-multi_objective_display>`
   * - Network iterations
     - :ref:`Network - Network Iterations <option-CPLEX-network_iterations>`
   * - Network netfind
     - :ref:`Network - Network Extraction Level <option-CPLEX-network_extraction_level>`
   * - Network pricing
     - :ref:`Network - Network Pricing <option-CPLEX-network_pricing>`
   * - Network tolerances feasibility
     - :ref:`Network - Network Feasibility <option-CPLEX-network_feasibility>`
   * - Network tolerances optimality
     - :ref:`Network - Network Optimality <option-CPLEX-network_optimality>`
   * - Optimalitytarget
     - :ref:`QP - Solution Target <option-CPLEX-solution_target>`
   * - Output clonelog
     - :ref:`Logging - Clone Log Files <option-CPLEX-clone_log_files>`
   * - Parallel mode
     - :ref:`Parallel - Parallel Mode <option-CPLEX-parallel_mode>`
   * - Paramdisplay
     - :ref:`Logging - Parameter Display <option-CPLEX-parameter_display>`
   * - Preprocessing aggregator
     - :ref:`Preprocessing - Aggregator <option-CPLEX-aggregator>`
   * - Preprocessing boundstrength
     - :ref:`MIP Preprocessing - Boundstrength <option-CPLEX-boundstrength>`
   * - Preprocessing coeffreduce
     - :ref:`MIP Preprocessing - Coefficient Reduction <option-CPLEX-coefficient_reduction>`
   * - Preprocessing dependency
     - :ref:`Preprocessing - Dependency <option-CPLEX-dependency>`
   * - Preprocessing dual
     - :ref:`Preprocessing - Presolve Pass Dual <option-CPLEX-presolve_pass_dual>`
   * - Preprocessing fill
     - :ref:`Preprocessing - Limit Substitutions <option-CPLEX-limit_substitutions>`
   * - Preprocessing folding
     - :ref:`Preprocessing - Folding <option-CPLEX-folding>`
   * - Preprocessing numpass
     - :ref:`Preprocessing - Number of Iterations in Presolve <option-CPLEX-number_of_iterations_in_presolve>`
   * - Preprocessing presolve
     - :ref:`Preprocessing - Presolve <option-CPLEX-presolve>`
   * - Preprocessing qcpduals
     - :ref:`QP - QCP Dual Values <option-CPLEX-qcp_dual_values>`
   * - Preprocessing qpmakepsd
     - :ref:`QP - Adjust MIQP <option-CPLEX-adjust_miqp>`
   * - Preprocessing qtolin
     - :ref:`QP - QP Linearization <option-CPLEX-qp_linearization>`
   * - Preprocessing reduce
     - :ref:`Preprocessing - Preprocessing Reduction Types <option-CPLEX-preprocessing_reduction_types>`
   * - Preprocessing relax
     - :ref:`MIP Preprocessing - Presolve Relaxed MIP <option-CPLEX-presolve_relaxed_mip>`
   * - Preprocessing repeatpresolve
     - :ref:`MIP Preprocessing - Repeat Presolve <option-CPLEX-repeat_presolve>`
   * - Preprocessing sos1reform
     - :ref:`MIP Preprocessing - SOS1 Reformulations <option-CPLEX-sos1_reformulations>`
   * - Preprocessing sos2reform
     - :ref:`MIP Preprocessing - SOS2 Reformulations <option-CPLEX-sos2_reformulations>`
   * - Preprocessing symmetry
     - :ref:`MIP Preprocessing - Preprocessing Symmetry <option-CPLEX-preprocessing_symmetry>`
   * - QPMethod
     - :ref:`QP - QP Method <option-CPLEX-qp_method>`
   * - Randomseed
     - :ref:`General - Random Seed <option-CPLEX-random_seed>`
   * - Read datacheck
     - :ref:`General - Data Check and Modeling Assistance <option-CPLEX-data_check_and_modeling_assistance>`
   * - Read qpnonzeros
     - :ref:`QP - QP Nonzeros Read Limit <option-CPLEX-qp_nonzeros_read_limit>`
   * - Read scale
     - :ref:`General - Scale <option-CPLEX-scale>`
   * - Sifting algorithm
     - :ref:`General - Sifting Algorithm <option-CPLEX-sifting_algorithm>`
   * - Sifting simplex
     - :ref:`Simplex - Sifting From Simplex <option-CPLEX-sifting_from_simplex>`
   * - Simplex crash
     - :ref:`Simplex - Crash Ordering <option-CPLEX-crash_ordering>`
   * - Simplex dgradient
     - :ref:`Simplex - Dual Pricing Algorithm <option-CPLEX-dual_pricing_algorithm>`
   * - Simplex display
     - :ref:`Logging - Simplex Display <option-CPLEX-simplex_display>`
   * - Simplex dynamicrows
     - :ref:`Simplex - Dynamic Row Management <option-CPLEX-dynamic_row_management>`
   * - Simplex limits iterations
     - :ref:`Stop Criteria - Iteration Limit <option-AIMMS-iteration_limit>`
   * - Simplex limits perturbation
     - :ref:`Simplex - Stalled Iterations <option-CPLEX-stalled_iterations>`
   * - Simplex limits singularity
     - :ref:`Simplex - Singular <option-CPLEX-singular>`
   * - Simplex perturbationlimit
     - :ref:`Simplex - Perturbation Constant <option-CPLEX-perturbation_constant>`
   * - Simplex perturbationlimit
     - :ref:`Simplex - Perturbation Indicator <option-CPLEX-perturbation_indicator>`
   * - Simplex pgradient
     - :ref:`Simplex - Primal Pricing Algorithm <option-CPLEX-primal_pricing_algorithm>`
   * - Simplex pricing
     - :ref:`Simplex - Pricing <option-CPLEX-pricing>`
   * - Simplex refactor
     - :ref:`Simplex - Refactor <option-CPLEX-refactor>`
   * - Simplex tolerances feasibility
     - :ref:`Simplex - Feasibility <option-CPLEX-feasibility>`
   * - Simplex tolerances markowitz
     - :ref:`Simplex - Markowitz <option-CPLEX-markowitz>`
   * - Simplex tolerances optimality
     - :ref:`Simplex - Optimality <option-CPLEX-optimality>`
   * - Solutiontype
     - :ref:`General - Solution Type <option-CPLEX-solution_type>`
   * - Threads
     - :ref:`Parallel - Global Thread Limit <option-CPLEX-global_thread_limit>`
   * - Timelimit
     - :ref:`Stop Criteria - Time Limit <option-AIMMS-time_limit>`
   * - Tune dettimelimit
     - :ref:`Tuning - Tuning Time Limit Deterministic <option-CPLEX-tuning_time_limit_deterministic>`
   * - Tune display
     - :ref:`Logging - Tuning Display <option-CPLEX-tuning_display>`
   * - Tune measure
     - :ref:`Tuning - Tuning Measure <option-CPLEX-tuning_measure>`
   * - Tune repeat
     - :ref:`Tuning - Tuning Repeater <option-CPLEX-tuning_repeater>`
   * - Tune timelimit
     - :ref:`Tuning - Tuning Time Limit <option-CPLEX-tuning_time_limit>`
   * - Workmem
     - :ref:`MIP - Working Memory Limit <option-CPLEX-working_memory_limit>`
