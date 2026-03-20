

.. _AIMMS_to_ODH_Mapping:


AIMMS to ODH Mapping
========================

**ODH engine options** 

The table below shows in the left column the AIMMS options that control the ODH engine; the right column displays for each AIMMS options the associated ODH-CPLEX parameter.

.. list-table::

   * - **Option name in AIMMS** 
     - **Name in ODH-CPLEX** 
   * - :ref:`Advanced - Backtrack Limit <option-ODHCPLEX-backtrack_limit>` 
     - MAXBACKTRACK
   * - :ref:`Advanced - Decomposition Density <option-ODHCPLEX-decomposition_density>` 
     - DECOMPDENSITY
   * - :ref:`Advanced - Global Bounds <option-ODHCPLEX-global_bounds>` 
     - GLOBALBOUNDS
   * - :ref:`Advanced - Initial Divisor Value <option-ODHCPLEX-initial_divisor_value>` 
     - INTERDIV
   * - :ref:`Advanced - Initial Divisor Value Sub Models <option-ODHCPLEX-initial_divisor_value_sub_models>` 
     - DIVISOR
   * - :ref:`Advanced - Maximum Divisor Repeats <option-ODHCPLEX-maximum_divisor_repeats>` 
     - MAXREPEAT
   * - :ref:`Advanced - Maximum Divisor Repeats Infeasible <option-ODHCPLEX-maximum_divisor_repeats_infeasible>` 
     - MAXINFREPEAT
   * - :ref:`Advanced - Maximum Divisor Value <option-ODHCPLEX-maximum_divisor_value>` 
     - MAXINTERDIV
   * - :ref:`Advanced - Optimization Method <option-ODHCPLEX-optimization_method>` 
     - FEASOPT
   * - :ref:`Advanced - Write Decomposition File <option-ODHCPLEX-write_decomposition_file>` 
     - 
   * - :ref:`General - Clean Variables Sub Models <option-ODHCPLEX-clean_variables_sub_models>` 
     - VARIABLECLEAN
   * - :ref:`General - Objective Target <option-ODHCPLEX-objective_target>` 
     - OBJTARGET
   * - :ref:`General - ODH Feasibility Tolerance <option-ODHCPLEX-odh_feasibility_tolerance>` 
     - FEASTOL
   * - :ref:`General - ODH Presolve <option-ODHCPLEX-odh_presolve>` 
     - ODHPRESOLVE
   * - :ref:`General - ODH Seed <option-ODHCPLEX-odh_seed>` 
     - SEED
   * - :ref:`General - Presolve <option-ODHCPLEX-presolve>` 
     - PRESOLVE
   * - :ref:`General - Quick First Solve <option-ODHCPLEX-quick_first_solve>` 
     - QUICKFIRSTSOLVE
   * - :ref:`General - Reject Infeasible Solutions <option-ODHCPLEX-reject_infeasible_solutions>` 
     - REJECTINFSOL
   * - :ref:`General - Relax SOS2 <option-ODHCPLEX-relax_sos2>` 
     - RELAXSOS2
   * - :ref:`General - Remove Infeasibilities Method <option-ODHCPLEX-remove_infeasibilities_method>` 
     - PHASE12
   * - :ref:`General - Search Mode <option-ODHCPLEX-search_mode>` 
     - 
   * - :ref:`General - Write Solution File <option-ODHCPLEX-write_solution_file>` 
     - WRITESOLUTION
   * - :ref:`Heuristics - First Feasible Heuristic <option-ODHCPLEX-first_feasible_heuristic>` 
     - FIRSTFEAS
   * - :ref:`Heuristics - First Feasible Heuristic Continue <option-ODHCPLEX-first_feasible_heuristic_continue>` 
     - FIRSTFEASCONTINUE
   * - :ref:`Heuristics - First Feasible Heuristic Effort Level <option-ODHCPLEX-first_feasible_heuristic_effort_level>` 
     - FIRSTFEASEFFORT
   * - :ref:`Heuristics - First Feasible Heuristic Shift <option-ODHCPLEX-first_feasible_heuristic_shift>` 
     - FIRSTFEASSHIFT
   * - :ref:`Heuristics - Recurse <option-ODHCPLEX-recurse>` 
     - RECURSE
   * - :ref:`Heuristics - Recurse Decomposition Method <option-ODHCPLEX-recurse_decomposition_method>` 
     - RECURSEDECOMP
   * - :ref:`Heuristics - Recurse Iteration Limit <option-ODHCPLEX-recurse_iteration_limit>` 
     - RECURSEITERLIM
   * - :ref:`Heuristics - Recurse Iteration Limit Solution <option-ODHCPLEX-recurse_iteration_limit_solution>` 
     - RECURSESOLITERLIM
   * - :ref:`Heuristics - Recurse Minimum Iterations <option-ODHCPLEX-recurse_minimum_iterations>` 
     - RECURSEMINITERLIM
   * - :ref:`Heuristics - Solution Improvement Heuristic Mode <option-ODHCPLEX-solution_improvement_heuristic_mode>` 
     - DETERMINISTIC
   * - :ref:`Heuristics - Solution Improvement Heuristic Penalty <option-ODHCPLEX-solution_improvement_heuristic_penalty>` 
     - PENALTY
   * - :ref:`Heuristics - Solution Improvement Heuristic Strategy <option-ODHCPLEX-solution_improvement_heuristic_strategy>` 
     - STRATEGY
   * - :ref:`Logging - Recurse Log <option-ODHCPLEX-recurse_log>` 
     - RECURSELOG
   * - :ref:`Logging - Status Display <option-ODHCPLEX-status_display>` 
     - 
   * - :ref:`Logging - Thread Log <option-ODHCPLEX-thread_log>` 
     - THREADLOG
   * - :ref:`Parallel - Thread Limit <option-ODHCPLEX-thread_limit>` 
     - THREADS
   * - :ref:`Parallel - Thread Synchronization Frequency <option-ODHCPLEX-thread_synchronization_frequency>` 
     - SYNCFREQ
   * - :ref:`Parallel - Processor Lock <option-ODHCPLEX-processor_lock>` 
     - PROCESSORLOCK






**CPLEX solve options** 

The two tables below show options used by ODH-CPLEX for the main CPLEX solve in ODH-CPLEX (if the **Search Mode**  is set to 'Global Solution') or for getting an initial feasible solution (if the **Search Mode**  is set to 'Local Solution').




.. list-table::

   * - **Option name in AIMMS** 
     - **Name in ODH-CPLEX for main CPLEX solve** 
   * - :ref:`CPLEX Barrier - Barrier Algorithm <option-ODHCPLEX-barrier_algorithm>`  
     - CPX_BARALG
   * - :ref:`CPLEX Barrier - Barrier Convergence Tolerance <option-ODHCPLEX-barrier_convergence_tolerance>`  
     - CPX_BAREPCOMP
   * - :ref:`CPLEX Barrier - Barrier Crossover Algorithm <option-ODHCPLEX-barrier_crossover_algorithm>` 
     - CPX_BARCROSSALG
   * - :ref:`CPLEX Barrier - Barrier Density Definition <option-ODHCPLEX-barrier_density_definition>`  
     - CPX_BARCOLNZ
   * - :ref:`CPLEX Barrier - Barrier Growth Limit <option-ODHCPLEX-barrier_growth_limit>`  
     - CPX_BARGROWTH
   * - :ref:`CPLEX Barrier - Barrier Iterations <option-ODHCPLEX-barrier_iterations>`  
     - CPX_BARITLIM
   * - :ref:`CPLEX Barrier - Barrier Maximal Number of Corrections <option-ODHCPLEX-barrier_maximal_number_of_corrections>`  
     - CPX_BARMAXCOR
   * - :ref:`CPLEX Barrier - Barrier Objective Range <option-ODHCPLEX-barrier_objective_range>`  
     - CPX_BAROBJRNG
   * - :ref:`CPLEX Barrier - Barrier Ordering <option-ODHCPLEX-barrier_ordering>`  
     - CPX_BARORDER
   * - :ref:`CPLEX Barrier - Barrier Start Algorithm <option-ODHCPLEX-barrier_start_algorithm>`  
     - CPX_BARSTARTALG
   * - :ref:`CPLEX General - Advanced Start <option-ODHCPLEX-advanced_start>` 
     - CPX_ADVIND
   * - :ref:`CPLEX General - Cleanup Coefficients <option-ODHCPLEX-cleanup_coefficients>` 
     - 
   * - :ref:`CPLEX General - Clock Type <option-ODHCPLEX-clock_type>` 
     - CPX_CLOCKTYPE
   * - :ref:`CPLEX General - Conflict Algorithm <option-ODHCPLEX-conflict_algorithm>`  
     - CPX_CONFLICTALG
   * - :ref:`CPLEX General - Data Check and Modeling Assistance <option-ODHCPLEX-data_check_and_modeling_assistance>`  
     - CPX_DATACHECK
   * - :ref:`CPLEX General - Deterministic Time Limit <option-ODHCPLEX-deterministic_time_limit>` 
     - CPX_DETTILIM
   * - :ref:`CPLEX General - LP File <option-ODHCPLEX-lp_file>`  
     - 
   * - :ref:`CPLEX General - Memory Emphasis <option-ODHCPLEX-memory_emphasis>` 
     - CPX_MEMORYEMPHASIS
   * - :ref:`CPLEX General - MPS <option-ODHCPLEX-mps>`  
     - 
   * - :ref:`CPLEX General - Numerical Emphasis <option-ODHCPLEX-numerical_emphasis>` 
     - CPX_NUMERICALEMPHASIS
   * - :ref:`CPLEX General - Ord File <option-ODHCPLEX-ord_file>`  
     - 
   * - :ref:`CPLEX General - Random Seed <option-ODHCPLEX-random_seed>`  
     - CPX_RANDOMSEED
   * - :ref:`CPLEX General - Round Coefficients <option-ODHCPLEX-round_coefficients>` 
     - 
   * - :ref:`CPLEX General - Sav File <option-ODHCPLEX-sav_file>`  
     - 
   * - :ref:`CPLEX General - Scale <option-ODHCPLEX-scale>`
     - CPX_SCAIND
   * - :ref:`CPLEX General - Sifting Algorithm <option-ODHCPLEX-sifting_algorithm>` 
     - CPX_SIFTALG
   * - :ref:`CPLEX General - Updates Batch Size <option-ODHCPLEX-updates_batch_size>`  
     - 
   * - :ref:`CPLEX Logging - Barrier Display <option-ODHCPLEX-barrier_display>`  
     - CPX_BARDISPLAY
   * - :ref:`CPLEX Logging - Clone Log Files <option-ODHCPLEX-clone_log_files>` 
     - CPX_CLONELOG
   * - :ref:`CPLEX Logging - MIP Display <option-ODHCPLEX-mip_display>`  
     - CPX_MIPDISPLAY
   * - :ref:`CPLEX Logging - MIP Interval <option-ODHCPLEX-mip_interval>` 
     - CPX_MIPINTERVAL
   * - :ref:`CPLEX Logging - Simplex Display <option-ODHCPLEX-simplex_display>`  
     - CPX_SIMDISPLAY
   * - :ref:`CPLEX MIP - Backtrack <option-ODHCPLEX-backtrack>`  
     - CPX_BTTOL
   * - :ref:`CPLEX MIP - Branch <option-ODHCPLEX-branch>`  
     - CPX_BRDIR
   * - :ref:`CPLEX MIP - Difference Objective <option-ODHCPLEX-difference_objective>`  
     - CPX_OBJDIF
   * - :ref:`CPLEX MIP - Integrality <option-ODHCPLEX-integrality>`  
     - CPX_EPINT
   * - :ref:`CPLEX MIP - Maximal Number of Nodes <option-ODHCPLEX-maximal_number_of_nodes>`  
     - CPX_NODELIM
   * - :ref:`CPLEX MIP - MIP Basis <option-ODHCPLEX-mip_basis>`  
     - 
   * - :ref:`CPLEX MIP - MIP Candidate List <option-ODHCPLEX-mip_candidate_list>` 
     - CPX_STRONGCANDLIM
   * - :ref:`CPLEX MIP - MIP Dive Strategy <option-ODHCPLEX-mip_dive_strategy>`  
     - CPX_DIVETYPE
   * - :ref:`CPLEX MIP - MIP Emphasis <option-ODHCPLEX-mip_emphasis>` 
     - CPX_MIPEMPHASIS
   * - :ref:`CPLEX MIP - MIP Method <option-ODHCPLEX-mip_method>`  
     - CPX_SUBALG
   * - :ref:`CPLEX MIP - MIP Probing <option-ODHCPLEX-mip_probing>` 
     - CPX_PROBE
   * - :ref:`CPLEX MIP - MIP Search Strategy <option-ODHCPLEX-mip_search_strategy>` 
     - CPX_MIPSEARCH
   * - :ref:`CPLEX MIP - MIP Start Algorithm <option-ODHCPLEX-mip_start_algorithm>`  
     - CPX_STARTALG
   * - :ref:`CPLEX MIP - MIP Tree Memory Limit <option-ODHCPLEX-mip_tree_memory_limit>`  
     - CPX_TRELIM
   * - :ref:`CPLEX MIP - MIP Update <option-ODHCPLEX-mip_update>`  
     - 
   * - :ref:`CPLEX MIP - Node File <option-ODHCPLEX-node_file>`  
     - CPX_NODEFILEIND
   * - :ref:`CPLEX MIP - MIP Node Presolve <option-ODHCPLEX-mip_node_presolve>`  
     - CPX_PRESLVND
   * - :ref:`CPLEX MIP - Number of Parallel Threads <option-ODHCPLEX-number_of_parallel_threads>` 
     - CPX_STRONGTHREADLIM
   * - :ref:`CPLEX MIP - Number of Repair Attempts <option-ODHCPLEX-number_of_repair_attempts>` 
     - CPX_REPAIRTRIES
   * - :ref:`CPLEX MIP - Number of Simplex Iterations <option-ODHCPLEX-number_of_simplex_iterations>`
     - CPX_STRONGITLIM
   * - :ref:`CPLEX MIP - MIP Priority Order Switch <option-ODHCPLEX-mip_priority_order_switch>`
     - CPX_MIPORDIND
   * - :ref:`CPLEX MIP - MIP Priority Order Type <option-ODHCPLEX-mip_priority_order_type>` 
     - CPX_MIPORDTYPE
   * - :ref:`CPLEX MIP - Probing Time <option-ODHCPLEX-probing_time>`  
     - CPX_PROBETIME
   * - :ref:`CPLEX MIP - Probing Time Deterministic <option-ODHCPLEX-probing_time_deterministic>`  
     - CPX_PROBEDETTIME
   * - :ref:`CPLEX MIP - Relative Difference Objective <option-ODHCPLEX-relative_difference_objective>`  
     - CPX_RELOBJDIF
   * - :ref:`CPLEX MIP - Select Variables <option-ODHCPLEX-select_variables>`  
     - CPX_VARSEL
   * - :ref:`CPLEX MIP - Selection of Nodes <option-ODHCPLEX-selection_of_nodes>`  
     - CPX_NODESEL
   * - :ref:`CPLEX MIP - Working Memory Limit <option-ODHCPLEX-working_memory_limit>`  
     - CPX_WORKMEM
   * - :ref:`CPLEX MIP - Write MIP Starts <option-ODHCPLEX-write_mip_starts>`  
     - 
   * - :ref:`CPLEX MIP Advanced - SubMIP Node Limit <option-ODHCPLEX-submip_node_limit>` 
     - CPX_SUBMIPNODELIMIT
   * - :ref:`CPLEX MIP Advanced - SubMIP Scale <option-ODHCPLEX-submip_scale>` 
     - CPX_SUBMIPSCAIND
   * - :ref:`CPLEX MIP Advanced - SubMIP Start Algorithm <option-ODHCPLEX-submip_start_algorithm>` 
     - CPX_SUBMIPSTARTALG
   * - :ref:`CPLEX MIP Advanced - SubMIP Subproblem Algorithm <option-ODHCPLEX-submip_subproblem_algorithm>` 
     - CPX_SUBMIPSUBALG
   * - :ref:`CPLEX MIP Cuts - BQP Cuts <option-ODHCPLEX-bqp_cuts>`  
     - CPX_BQPCUTS
   * - :ref:`CPLEX MIP Cuts - Clique Cuts <option-ODHCPLEX-clique_cuts>`  
     - CPX_CLIQUES
   * - :ref:`CPLEX MIP Cuts - Cover Cuts <option-ODHCPLEX-cover_cuts>` 
     - CPX_COVERS
   * - :ref:`CPLEX MIP Cuts - Cut Generation Limit <option-ODHCPLEX-cut_generation_limit>` 
     - CPX_AGGCUTLIM
   * - :ref:`CPLEX MIP Cuts - Cut Limit <option-ODHCPLEX-cut_limit>`  
     - CPX_EACHCUTLIM
   * - :ref:`CPLEX MIP Cuts - Cuts Factor <option-ODHCPLEX-cuts_factor>`  
     - CPX_CUTSFACTOR
   * - :ref:`CPLEX MIP Cuts - Disjunctive Cuts <option-ODHCPLEX-disjunctive_cuts>` 
     - CPX_DISJCUTS
   * - :ref:`CPLEX MIP Cuts - Flow Cover Cuts <option-ODHCPLEX-flow_cover_cuts>` 
     - CPX_FLOWCOVERS
   * - :ref:`CPLEX MIP Cuts - Flow Path Cuts <option-ODHCPLEX-flow_path_cuts>` 
     - CPX_FLOWPATHS
   * - :ref:`CPLEX MIP Cuts - Gomory Cuts <option-ODHCPLEX-gomory_cuts>` 
     - CPX_FRACCUTS
   * - :ref:`CPLEX MIP Cuts - Gomory Cuts Candidate Limit <option-ODHCPLEX-gomory_cuts_candidate_limit>` 
     - CPX_FRACCAND
   * - :ref:`CPLEX MIP Cuts - Gomory Cuts Pass Limit <option-ODHCPLEX-gomory_cuts_pass_limit>` 
     - CPX_FRACPASS
   * - :ref:`CPLEX MIP Cuts - GUB Cover Cuts <option-ODHCPLEX-gub_cover_cuts>` 
     - CPX_GUBCOVERS
   * - :ref:`CPLEX MIP Cuts - Implied Bound Cuts <option-ODHCPLEX-implied_bound_cuts>` 
     - CPX_IMPLBD
   * - :ref:`CPLEX MIP Cuts - Lift and Project Cuts <option-ODHCPLEX-lift_and_project_cuts>` 
     - CPX_LANDPCUTS
   * - :ref:`CPLEX MIP Cuts - Local Implied Bound Cuts <option-ODHCPLEX-local_implied_bound_cuts>` 
     - CPX_LOCALIMPLBD
   * - :ref:`CPLEX MIP Cuts - MCF Cuts <option-ODHCPLEX-mcf_cuts>`  
     - CPX_MCFCUTS
   * - :ref:`CPLEX MIP Cuts - MIP Number of Cut Passes <option-ODHCPLEX-mip_number_of_cut_passes>` 
     - CPX_CUTPASS
   * - :ref:`CPLEX MIP Cuts - Mixed Integer Rounding Cuts <option-ODHCPLEX-mixed_integer_rounding_cuts>`  
     - CPX_MIRCUTS
   * - :ref:`CPLEX MIP Cuts - Node Cuts <option-ODHCPLEX-node_cuts>`  
     - CPX_NODECUTS
   * - :ref:`CPLEX MIP Cuts - RLT Cuts <option-ODHCPLEX-rlt_cuts>`  
     - CPX_RLTCUTS
   * - :ref:`CPLEX MIP Cuts - Zero Half Cuts <option-ODHCPLEX-zero_half_cuts>`  
     - CPX_ZEROHALFCUTS
   * - :ref:`CPLEX MIP Heuristics - Feasibility Pump Heuristic <option-ODHCPLEX-feasibility_pump_heuristic>` 
     - CPX_FPHEUR
   * - :ref:`CPLEX MIP Heuristics - Heuristic Effort <option-ODHCPLEX-heuristic_effort>` 
     - CPX_HEUREFFORT
   * - :ref:`CPLEX MIP Heuristics - Heuristic Frequency <option-ODHCPLEX-heuristic_frequency>` 
     - CPX_HEURFREQ
   * - :ref:`CPLEX MIP Heuristics - Local Branching Heuristic <option-ODHCPLEX-local_branching_heuristic>`  
     - CPX_LBHEUR
   * - :ref:`CPLEX MIP Heuristics - RINS Heuristic Frequency <option-ODHCPLEX-rins_heuristic_frequency>` 
     - CPX_RINSHEUR
   * - :ref:`CPLEX MIP Preprocessing - Boundstrength <option-ODHCPLEX-boundstrength>`  
     - CPX_BNDSTRENIND
   * - :ref:`CPLEX MIP Preprocessing - Coefficient Reduction <option-ODHCPLEX-coefficient_reduction>` 
     - CPX_COEREDIND
   * - :ref:`CPLEX MIP Preprocessing - Preprocessing Symmetry <option-ODHCPLEX-preprocessing_symmetry>`  
     - CPX_SYMMETRY
   * - :ref:`CPLEX MIP Preprocessing - Presolve Relaxed MIP <option-ODHCPLEX-presolve_relaxed_mip>`  
     - CPX_RELAXPREIND
   * - :ref:`CPLEX MIP Preprocessing - Repeat Presolve <option-ODHCPLEX-repeat_presolve>`  
     - CPX_REPEATPRESOLVE
   * - :ref:`CPLEX MIP Preprocessing - SOS1 Reformulations <option-ODHCPLEX-sos1_reformulations>` 
     - CPX_SOS1REFORM
   * - :ref:`CPLEX MIP Preprocessing - SOS2 Reformulations <option-ODHCPLEX-sos2_reformulations>` 
     - CPX_SOS2REFORM
   * - :ref:`CPLEX MIP Solution Polishing - Polishing Absolute MIP Gap <option-ODHCPLEX-polishing_absolute_mip_gap>`  
     - CPX_POLISHAFTEREPAGAP
   * - :ref:`CPLEX MIP Solution Polishing - Polishing Number of Nodes <option-ODHCPLEX-polishing_number_of_nodes>`  
     - CPX_POLISHAFTERNODE
   * - :ref:`CPLEX MIP Solution Polishing - Polishing Number of Solutions <option-ODHCPLEX-polishing_number_of_solutions>`  
     - CPX_POLISHAFTERINTSOL
   * - :ref:`CPLEX MIP Solution Polishing - Polishing Relative MIP Gap <option-ODHCPLEX-polishing_relative_mip_gap>`  
     - CPX_POLISHAFTEREPGAP
   * - :ref:`CPLEX MIP Solution Polishing - Polishing Time <option-ODHCPLEX-polishing_time>`  
     - CPX_POLISHAFTERTIME
   * - :ref:`CPLEX MIP Solution Polishing - Polishing Time Deterministic <option-ODHCPLEX-polishing_time_deterministic>`  
     - CPX_POLISHAFTERDETTIME
   * - :ref:`CPLEX MIP Solution Pool - Do Populate <option-ODHCPLEX-do_populate>`  
     - 
   * - :ref:`CPLEX MIP Solution Pool - Pool Absolute Objective Gap <option-ODHCPLEX-pool_absolute_objective_gap>` 
     - CPX_SOLNPOOLAGAP
   * - :ref:`CPLEX MIP Solution Pool - Pool Capacity <option-ODHCPLEX-pool_capacity>`  
     - CPX_SOLNPOOLCAPACITY
   * - :ref:`CPLEX MIP Solution Pool - Pool Intensity <option-ODHCPLEX-pool_intensity>`  
     - CPX_SOLNPOOLINTENSITY
   * - :ref:`CPLEX MIP Solution Pool - Pool Relative Objective Gap <option-ODHCPLEX-pool_relative_objective_gap>` 
     - CPX_SOLNPOOLGAP
   * - :ref:`CPLEX MIP Solution Pool - Pool Replacement Strategy <option-ODHCPLEX-pool_replacement_strategy>`  
     - CPX_SOLNPOOLREPLACE
   * - :ref:`CPLEX MIP Solution Pool - Populate Time Limit <option-ODHCPLEX-populate_time_limit>`  
     - 
   * - :ref:`CPLEX MIP Solution Pool - Population Limit <option-ODHCPLEX-population_limit>`  
     - CPX_POPULATELIM
   * - :ref:`CPLEX Network - Network Feasibility <option-ODHCPLEX-network_feasibility>` 
     - CPX_NETEPRHS
   * - :ref:`CPLEX Network - Network Iterations <option-ODHCPLEX-network_iterations>` 
     - CPX_NETITLIM
   * - :ref:`CPLEX Network - Network Optimality <option-ODHCPLEX-network_optimality>` 
     - CPX_NETEPOPT
   * - :ref:`CPLEX Network - Network Pricing <option-ODHCPLEX-network_pricing>` 
     - CPX_NETPPRIIND
   * - :ref:`CPLEX Parallel - Auxiliary Root Threads <option-ODHCPLEX-auxiliary_root_threads>` 
     - CPX_AUXROOTTHREADS
   * - :ref:`CPLEX Parallel - Global Thread Limit <option-ODHCPLEX-global_thread_limit>` 
     - CPX_THREADS
   * - :ref:`CPLEX Parallel - Parallel Mode <option-ODHCPLEX-parallel_mode>` 
     - CPX_PARALLELMODE
   * - :ref:`CPLEX Preprocessing - Aggregator <option-ODHCPLEX-aggregator>` 
     - CPX_AGGIND
   * - :ref:`CPLEX Preprocessing - Dependency <option-ODHCPLEX-dependency>`
     - CPX_DEPIND
   * - :ref:`CPLEX Preprocessing - Folding <option-ODHCPLEX-folding>` 
     - CPX_FOLDING
   * - :ref:`CPLEX Preprocessing - Limit Substitutions <option-ODHCPLEX-limit_substitutions>`  
     - CPX_AGGFILL
   * - :ref:`CPLEX Preprocessing - Number of Iterations in Presolve <option-ODHCPLEX-number_of_iterations_in_presolve>` 
     - CPX_PREPASS
   * - :ref:`CPLEX Preprocessing - Preprocessing Reduction Types <option-ODHCPLEX-preprocessing_reduction_types>`  
     - CPX_REDUCE
   * - :ref:`CPLEX Preprocessing - Presolve Pass Dual <option-ODHCPLEX-presolve_pass_dual>` 
     - CPX_PREDUAL
   * - :ref:`CPLEX Quadratic - Adjust MIQP <option-ODHCPLEX-adjust_miqp>`  
     - CPX_QPMAKEPSDIND
   * - :ref:`CPLEX Quadratic - Barrier Convergence Tolerance for QCP <option-ODHCPLEX-barrier_convergence_tolerance_for_qcp>`  
     - CPX_BARQCPEPCOMP
   * - :ref:`CPLEX Quadratic - MIQCP Strategy <option-ODHCPLEX-miqcp_strategy>`  
     - CPX_MIQCPSTRAT
   * - :ref:`CPLEX Quadratic - QP Linearization <option-ODHCPLEX-qp_linearization>`  
     - CPX_QTOLININD
   * - :ref:`CPLEX Quadratic - QP Method <option-ODHCPLEX-qp_method>`  
     - CPX_QPMETHOD
   * - :ref:`CPLEX Quadratic - QP Nonzeros Read Limit <option-ODHCPLEX-qp_nonzeros_read_limit>`  
     - CPX_QPNZREADLIM
   * - :ref:`CPLEX Quadratic - Solution Target <option-ODHCPLEX-solution_target>`  
     - CPX_OPTIMALITYTARGET
   * - :ref:`CPLEX Simplex - Crash Ordering <option-ODHCPLEX-crash_ordering>`  
     - CPX_CRAIND
   * - :ref:`CPLEX Simplex - Dual Pricing Algorithm <option-ODHCPLEX-dual_pricing_algorithm>`  
     - CPX_DPRIIND
   * - :ref:`CPLEX Simplex - Dynamic Row Management <option-ODHCPLEX-dynamic_row_management>` 
     - CPX_DYNAMICROWS
   * - :ref:`CPLEX Simplex - Feasibility <option-ODHCPLEX-feasibility>`  
     - CPX_EPRHS
   * - :ref:`CPLEX Simplex - Markowitz <option-ODHCPLEX-markowitz>` 
     - CPX_EPMRK
   * - :ref:`CPLEX Simplex - Optimality <option-ODHCPLEX-optimality>`  
     - CPX_EPOPT
   * - :ref:`CPLEX Simplex - Perturbation Constant <option-ODHCPLEX-perturbation_constant>`  
     - CPX_EPPER
   * - :ref:`CPLEX Simplex - Perturbation Indicator <option-ODHCPLEX-perturbation_indicator>` 
     - CPX_PERIND
   * - :ref:`CPLEX Simplex - Pricing <option-ODHCPLEX-pricing>`  
     - CPX_PRICELIM
   * - :ref:`CPLEX Simplex - Primal Pricing Algorithm <option-ODHCPLEX-primal_pricing_algorithm>`  
     - CPX_PPRIIND
   * - :ref:`CPLEX Simplex - Refactor <option-ODHCPLEX-refactor>`  
     - CPX_REINV
   * - :ref:`CPLEX Simplex - Sifting from Simplex <option-ODHCPLEX-sifting_from_simplex>` 
     - CPX_SIFTSIM
   * - :ref:`CPLEX Simplex - Singular <option-ODHCPLEX-singular>` 
     - CPX_SINGLIM
   * - :ref:`CPLEX Simplex - Stalled Iterations <option-ODHCPLEX-stalled_iterations>`  
     - CPX_PERLIM






The table below shows Solvers General options that are mapped to ODH-CPLEX parameters.




.. list-table::

   * - **Option name in AIMMS** 
     - **Name in ODH-CPLEX** 
   * - :ref:`MIP Options - Cutoff <option-AIMMS-cutoff>` 
     - CPX_CUTLO
   * - 
     - CPX_CUTUP
   * - :ref:`MIP Options - Maximal Number of Integer Solutions <option-AIMMS-maximal_number_of_integer_solutions>` 
     - CPX_INTSOLLIM
   * - :ref:`MIP Options - MIP Absolute Optimality Tolerance <option-AIMMS-mip_absolute_optimality_tolerance>` 
     - CPX_EPAGAP
   * - :ref:`MIP Options - MIP Relative Optimality Tolerance <option-AIMMS-mip_relative_optimality_tolerance>` 
     - CPX_EPGAP
   * - :ref:`Stop Criteria - Iteration Limit <option-AIMMS-iteration_limit>` 
     - CPX_ITLIM
   * - :ref:`Stop Criteria - Time Limit <option-AIMMS-time_limit>` 
     - TIMELIMIT






**Heuristic sub-model options** 

The heuristic sub-model parameters can only be set using a :ref:`ODH-CPLEX_-_Parameter_File`. The syntax for the parameters that influence the heuristic sub-model CPLEX solves is the following: SUB_<parameter> where <parameter> refers to the ODH-CPLEX name in the second table above. The syntax for the parameters that influence the heuristic sub-model CPLEX solves in Phase I is the following: PHASE1_<parameter>.



For example, SUB_CPX_RINSHEUR specifies the RINS heuristic frequency for CPLEX if it used to solve a heuristic sub-model, while PHASE1_CPX_RINSHEUR specifies the RINS heuristic frequency for CPLEX if it used to solve a heuristic sub-model in Phase I.



**Learn more about** 

*	:ref:`ODH-CPLEX_-_Parameter_File` 
*	:ref:`General - Search Mode <option-ODHCPLEX-search_mode>`  
