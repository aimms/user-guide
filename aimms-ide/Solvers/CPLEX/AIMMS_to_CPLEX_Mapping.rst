

.. _AIMMS_to_CPLEX_Mapping:


AIMMS to CPLEX Mapping
===========================

**Description** 

The table below shows in the left column the AIMMS CPLEX options; the middle column displays the CPLEX parameters that are associated with them. The right column displays the constants used in the CPLEX C API.

.. list-table::

   * - **Option name in AIMMS** 
     - **Name in CPLEX** 
     - **Name in CPLEX C API** 
   * - :ref:`Barrier - Barrier Algorithm <option-CPLEX-barrier_algorithm>`
     - Barrier algorithm
     - CPX_PARAM_BARALG
   * - :ref:`Barrier - Barrier Always <option-CPLEX-barrier_always>`
     - 
     - 
   * - :ref:`Barrier - Barrier Convergence Tolerance <option-CPLEX-barrier_convergence_tolerance>`
     - Barrier convergetol
     - CPX_PARAM_BAREPCOMP
   * - :ref:`Barrier - Barrier Crossover Algorithm <option-CPLEX-barrier_crossover_algorithm>`
     - Barrier crossover
     - CPX_PARAM_BARCROSSALG
   * - :ref:`Barrier - Barrier Density Definition <option-CPLEX-barrier_density_definition>`
     - Barrier colnonzeros
     - CPX_PARAM_BARCOLNZ
   * - :ref:`Barrier - Barrier Growth Limit <option-CPLEX-barrier_growth_limit>`
     - Barrier limits growth
     - CPX_PARAM_BARGROWTH
   * - :ref:`Barrier - Barrier Iterations <option-CPLEX-barrier_iterations>`
     - Barrier limits iteration
     - CPX_PARAM_BARITLIM
   * - :ref:`Barrier - Barrier Maximal Number of Corrections <option-CPLEX-barrier_maximal_number_of_corrections>`
     - Barrier limits corrections
     - CPX_PARAM_BARMAXCOR
   * - :ref:`Barrier - Barrier Objective Range <option-CPLEX-barrier_objective_range>`
     - Barrier limits objrange
     - CPX_PARAM_BAROBJRNG
   * - :ref:`Barrier - Barrier Ordering <option-CPLEX-barrier_ordering>`
     - Barrier ordering
     - CPX_PARAM_BARORDER
   * - :ref:`Barrier - Barrier Progress Solution <option-CPLEX-barrier_progress_solution>`
     - 
     - 
   * - :ref:`Barrier - Barrier Start Algorithm <option-CPLEX-barrier_start_algorithm>`
     - Barrier startalg
     - CPX_PARAM_BARSTARTALG
   * - :ref:`Benders - Benders Decomposition Check Limit <option-CPLEX-benders_decomposition_check_limit>`
     - 
     - 
   * - :ref:`Benders - Benders Feasibility Cut Tolerance <option-CPLEX-benders_feasibility_cut_tolerance>`
     - Benders tolerances feasibilitycut
     - CPX_PARAM_BENDERSFEASCUTTOL
   * - :ref:`Benders - Benders Optimality Cut Tolerance <option-CPLEX-benders_optimality_cut_tolerance>`
     - Benders tolerances optimalitycut
     - CPX_PARAM_BENDERSOPTCUTTOL
   * - :ref:`Benders - Benders Strategy <option-CPLEX-benders_strategy>`
     - Benders strategy
     - CPX_PARAM_BENDERSSTRATEGY
   * - :ref:`Benders - Benders Worker Algorithm <option-CPLEX-benders_worker_algorithm>`
     - Benders workeralgorithm
     - CPX_PARAM_WORKERALG
   * - :ref:`General - Advanced Start <option-CPLEX-advanced_start>`
     - Advance
     - CPX_PARAM_ADVIND
   * - :ref:`General - Check Solution <option-CPLEX-check_solution>`
     - 
     - 
   * - :ref:`General - Cleanup Coefficients <option-CPLEX-cleanup_coefficients>`
     - 
     - 
   * - :ref:`General - Clock Type <option-CPLEX-clock_type>`
     - Clocktype
     - CPX_PARAM_CLOCKTYPE
   * - :ref:`General - Cmd File <option-CPLEX-cmd_file>`
     - 
     - 
   * - :ref:`General - Conflict Algorithm <option-CPLEX-conflict_algorithm>`
     - Conflict algorithm
     - CPX_PARAM_CONFLICTALG
   * - :ref:`General - Data Check and Modeling Assistance <option-CPLEX-data_check_and_modeling_assistance>`
     - Read datacheck
     - CPX_PARAM_DATACHECK
   * - :ref:`General - Deterministic Time Limit <option-CPLEX-deterministic_time_limit>`
     - Dettimelimit
     - CPX_PARAM_DETTILIM
   * - :ref:`General - Display Solution Statistics <option-CPLEX-display_solution_statistics>`
     - 
     - 
   * - :ref:`General - Farkas Infeasibility Proof <option-CPLEX-farkas_infeasibility_proof>`
     - 
     - 
   * - :ref:`General - Feasopt Tolerance <option-CPLEX-feasopt_tolerance>`
     - Feasopt tolerance
     - CPX_PARAM_Feasopt_Tolerance
   * - :ref:`General - LP File <option-CPLEX-lp_file>`
     - 
     - 
   * - :ref:`General - LP Method <option-CPLEX-lp_method>`
     - Lpmethod
     - CPX_PARAM_LPMETHOD
   * - :ref:`General - Memory Emphasis <option-CPLEX-memory_emphasis>`
     - Emphasis memory
     - CPX_PARAM_MEMORYEMPHASIS
   * - :ref:`General - MPS <option-CPLEX-mps>`
     - 
     - 
   * - :ref:`General - Numerical Emphasis <option-CPLEX-numerical_emphasis>`
     - Emphasis numerical
     - CPX_PARAM_NUMERICALEMPHASIS
   * - :ref:`General - Ord File <option-CPLEX-ord_file>`
     - 
     - 
   * - :ref:`General - Random Seed <option-CPLEX-random_seed>`
     - Randomseed
     - CPX_PARAM_RANDOMSEED
   * - :ref:`General - Read Parameter File <option-CPLEX-read_parameter_file>`
     - 
     - 
   * - :ref:`General - Restart <option-CPLEX-restart>`
     - 
     - 
   * - :ref:`General - Restart File Number <option-CPLEX-restart_file_number>`
     - 
     - 
   * - :ref:`General - Round Coefficients <option-CPLEX-round_coefficients>`
     - 
     - 
   * - :ref:`General - Sav File <option-CPLEX-sav_file>`
     - 
     - 
   * - :ref:`General - Scale <option-CPLEX-scale>`
     - Read scale
     - CPX_PARAM_SCAIND
   * - :ref:`General - Sensitivity Method <option-CPLEX-sensitivity_method>`
     - 
     - 
   * - :ref:`General - Sifting Algorithm <option-CPLEX-sifting_algorithm>`
     - Sifting algorithm
     - CPX_PARAM_SIFTALG
   * - :ref:`General - Solution File <option-CPLEX-solution_file>`
     - 
     - 
   * - :ref:`General - Solution Type <option-CPLEX-solution_type>`
     - Solutiontype
     - CPX_PARAM_SOLUTIONTYPE
   * - :ref:`General - Stealth Mode <option-CPLEX-stealth_mode>`
     - 
     - 
   * - :ref:`General - Unbounded Ray <option-CPLEX-unbounded_ray>`
     - 
     - 
   * - :ref:`General - Updates Batch Size <option-CPLEX-updates_batch_size>`
     - 
     - 
   * - :ref:`General - Write Annotations File <option-CPLEX-write_annotations_file>`
     - 
     - 
   * - :ref:`General - Write Parameter File <option-CPLEX-write_parameter_file>`
     - 
     - 
   * - :ref:`Logging - Barrier Display <option-CPLEX-barrier_display>`
     - Barrier display
     - CPX_PARAM_BARDISPLAY
   * - :ref:`Logging - Clone Log Files <option-CPLEX-clone_log_files>`
     - Output clonelog
     - CPX_PARAM_CLONELOG
   * - :ref:`Logging - MIP Display <option-CPLEX-mip_display>`
     - MIP display
     - CPX_PARAM_MIPDISPLAY
   * - :ref:`Logging - MIP Interval <option-CPLEX-mip_interval>`
     - MIP interval
     - CPX_PARAM_MIPINTERVAL
   * - :ref:`Logging - Multi Objective Display <option-CPLEX-multi_objective_display>`
     - Multiobjective display 
     - CPX_PARAM_MULTIOBJDISPLAY
   * - :ref:`Logging - Parameter Display <option-CPLEX-parameter_display>`
     - Paramdisplay
     - CPX_PARAM_PARAMDISPLAY
   * - :ref:`Logging - Simplex Display <option-CPLEX-simplex_display>`
     - Simplex display
     - CPX_PARAM_SIMDISPLAY
   * - :ref:`Logging - Tuning Display <option-CPLEX-tuning_display>`
     - Tune display
     - CPX_PARAM_TUNINGDISPLAY
   * - :ref:`Logging - Backtrack <option-CPLEX-backtrack>`
     - MIP strategy backtrack
     - CPX_PARAM_BTTOL
   * - :ref:`MIP - Branch <option-CPLEX-branch>`
     - MIP strategy branch
     - CPX_PARAM_BRDIR
   * - :ref:`MIP - Difference Objective <option-CPLEX-difference_objective>`
     - MIP tolerances objdifference
     - CPX_PARAM_OBJDIF
   * - :ref:`MIP - Integrality <option-CPLEX-integrality>`
     - MIP tolerances integrality
     - CPX_PARAM_EPINT
   * - :ref:`MIP - Maximal Number of Nodes <option-CPLEX-maximal_number_of_nodes>`
     - MIP limits nodes
     - CPX_PARAM_NODELIM
   * - :ref:`MIP - MIP Basis <option-CPLEX-mip_basis>`
     - 
     - 
   * - :ref:`MIP - MIP Candidate List <option-CPLEX-mip_candidate_list>`
     - MIP limits strongcand
     - CPX_PARAM_STRONGCANDLIM
   * - :ref:`MIP - MIP Dive Strategy <option-CPLEX-mip_dive_strategy>`
     - MIP strategy dive
     - CPX_PARAM_DIVETYPE
   * - :ref:`MIP - MIP Emphasis <option-CPLEX-mip_emphasis>`
     - Emphasis MIP
     - CPX_PARAM_MIPEMPHASIS
   * - :ref:`MIP - MIP Kappa <option-CPLEX-mip_kappa>`
     - MIP strategy kappastats
     - CPX_PARAM_MIPKAPPASTATS
   * - :ref:`MIP - MIP Method <option-CPLEX-mip_method>`
     - MIP strategy subalgorithm
     - CPX_PARAM_SUBALG
   * - :ref:`MIP - MIP Priority Order Switch <option-CPLEX-mip_priority_order_switch>`
     - MIP strategy order
     - CPX_PARAM_MIPORDIND
   * - :ref:`MIP - MIP Priority Order Type <option-CPLEX-mip_priority_order_type>`
     - MIP ordertype
     - CPX_PARAM_MIPORDTYPE
   * - :ref:`MIP - MIP Probing <option-CPLEX-mip_probing>`
     - MIP strategy probe
     - CPX_PARAM_PROBE
   * - :ref:`MIP - MIP Search Strategy <option-CPLEX-mip_search_strategy>`
     - MIP strategy search
     - CPX_PARAM_MIPSEARCH
   * - :ref:`MIP - MIP Start Algorithm <option-CPLEX-mip_start_algorithm>`
     - MIP strategy startalgorithm
     - CPX_PARAM_STARTALG
   * - :ref:`MIP - MIP Tree Memory Limit <option-CPLEX-mip_tree_memory_limit>`
     - MIP limits treememory
     - CPX_PARAM_TRELIM
   * - :ref:`MIP - MIP Update <option-CPLEX-mip_update>`
     - 
     - 
   * - :ref:`MIP - Node File <option-CPLEX-node_file>`
     - MIP strategy file
     - CPX_PARAM_NODEFILEIND
   * - :ref:`MIP - MIP Node Presolve <option-CPLEX-mip_node_presolve>`
     - MIP strategy presolvenode
     - CPX_PARAM_PRESLVND
   * - :ref:`MIP - Number of Repair Attempts <option-CPLEX-number_of_repair_attempts>`
     - MIP limits repairtries
     - CPX_PARAM_REPAIRTRIES
   * - :ref:`MIP - Number of Simplex Iterations <option-CPLEX-number_of_simplex_iterations>`
     - MIP limits strongit
     - CPX_PARAM_STRONGITLIM
   * - :ref:`MIP - Probing Time <option-CPLEX-probing_time>`
     - MIP limits probetime
     - CPX_PARAM_PROBETIME
   * - :ref:`MIP - Probing Time Deterministic <option-CPLEX-probing_time_deterministic>`
     - MIP limits probedettime
     - CPX_PARAM_PROBEDETTIME
   * - :ref:`MIP - Relative Difference Objective <option-CPLEX-relative_difference_objective>`
     - MIP tolerances relobjdifference
     - CPX_PARAM_RELOBJDIF
   * - :ref:`MIP - Select Variables <option-CPLEX-select_variables>`
     - MIP strategy variableselect
     - CPX_PARAM_VARSEL
   * - :ref:`MIP - Selection of Nodes <option-CPLEX-selection_of_nodes>`
     - MIP strategy nodeselect
     - CPX_PARAM_NODESEL
   * - :ref:`MIP - Use Generic Callbacks <option-CPLEX-use_generic_callbacks>`
     - 
     - 
   * - :ref:`MIP - Working Memory Limit <option-CPLEX-working_memory_limit>`
     - Workmem
     - CPX_PARAM_WORKMEM
   * - :ref:`MIP - Write MIP Starts <option-CPLEX-write_mip_starts>`
     - 
     - 
   * - :ref:`MIP Advanced - Find Fractional Root Solution <option-CPLEX-find_fractional_root_solution>`
     - 
     - 
   * - :ref:`MIP Advanced - Lower Objective Stop <option-CPLEX-lower_objective_stop>`
     - MIP limits lowerobjstop
     - CPX_PARAM_LOWEROBJSTOP
   * - :ref:`MIP Advanced - SubMIP Node Limit <option-CPLEX-submip_node_limit>`
     - MIP submip nodelimit
     - CPX_PARAM_SUBMIPNODELIMIT
   * - :ref:`MIP Advanced - SubMIP Scale <option-CPLEX-submip_scale>`
     - MIP submip scale
     - CPX_PARAM_SUBMIPSCAIND
   * - :ref:`MIP Advanced - SubMIP Start Algorithm <option-CPLEX-submip_start_algorithm>`
     - MIP submip startalg
     - CPX_PARAM_SUBMIPSTARTALG
   * - :ref:`MIP Advanced - SubMIP Subproblem Algorithm <option-CPLEX-submip_subproblem_algorithm>`
     - MIP submip subalg
     - CPX_PARAM_SUBMIPSUBALG
   * - :ref:`MIP Advanced - Upper Objective Stop <option-CPLEX-upper_objective_stop>`
     - MIP limits upperobjstop
     - CPX_PARAM_UPPEROBJSTOP
   * - :ref:`MIP Advanced - Write Cuts <option-CPLEX-write_cuts>`
     - 
     - 
   * - :ref:`MIP Advanced - Write Cuts Variable Values <option-CPLEX-write_cuts_variable_values>`
     - 
     - 
   * - :ref:`MIP Cuts - Bqp Cuts <option-CPLEX-bqp_cuts>`
     - MIP cuts bqp
     - CPX_PARAM_BQPCUTS
   * - :ref:`MIP Cuts - Clique Cuts <option-CPLEX-clique_cuts>`
     - MIP cuts cliques
     - CPX_PARAM_CLIQUES
   * - :ref:`MIP Cuts - Cover Cuts <option-CPLEX-cover_cuts>`
     - MIP cuts covers
     - CPX_PARAM_COVERS
   * - :ref:`MIP Cuts - Cut Generation Limit <option-CPLEX-cut_generation_limit>`
     - MIP limits aggforcut
     - CPX_PARAM_AGGCUTLIM
   * - :ref:`MIP Cuts - Cut Limit <option-CPLEX-cut_limit>`
     - MIP limits eachcutlimit
     - CPX_PARAM_EACHCUTLIM
   * - :ref:`MIP Cuts - Cuts Factor <option-CPLEX-cuts_factor>`
     - MIP limits cutsfactor
     - CPX_PARAM_CUTSFACTOR
   * - :ref:`MIP Cuts - Disjunctive Cuts <option-CPLEX-disjunctive_cuts>`
     - MIP cuts disjunctive
     - CPX_PARAM_DISJCUTS
   * - :ref:`MIP Cuts - Flow Cover Cuts <option-CPLEX-flow_cover_cuts>`
     - MIP cuts flow
     - CPX_PARAM_FLOWCOVERS
   * - :ref:`MIP Cuts - Flow Path Cuts <option-CPLEX-flow_path_cuts>`
     - MIP cuts pathcut
     - CPX_PARAM_FLOWPATHS
   * - :ref:`MIP Cuts - Gomory Cuts <option-CPLEX-gomory_cuts>`
     - MIP cuts gomory
     - CPX_PARAM_FRACCUTS
   * - :ref:`MIP Cuts - Gomory Cuts Candidate Limit <option-CPLEX-gomory_cuts_candidate_limit>`
     - MIP limits gomorycand
     - CPX_PARAM_FRACCAND
   * - :ref:`MIP Cuts - Gomory Cuts Pass Limit <option-CPLEX-gomory_cuts_pass_limit>`
     - MIP limits gomorypass
     - CPX_PARAM_FRACPASS
   * - :ref:`MIP Cuts - Gub Cover Cuts <option-CPLEX-gub_cover_cuts>`
     - MIP cuts gubcovers
     - CPX_PARAM_GUBCOVERS
   * - :ref:`MIP Cuts - Implied Bound Cuts <option-CPLEX-implied_bound_cuts>`
     - MIP cuts implied
     - CPX_PARAM_IMPLBD
   * - :ref:`MIP Cuts - Lift and Project Cuts <option-CPLEX-lift_and_project_cuts>`
     - MIP cuts liftproj
     - CPX_PARAM_LANDPCUTS
   * - :ref:`MIP Cuts - Local Implied Bound Cuts <option-CPLEX-local_implied_bound_cuts>`
     - MIP cuts localimplied
     - CPX_PARAM_LOCALIMPLBD
   * - :ref:`MIP Cuts - MCF Cuts <option-CPLEX-mcf_cuts>`
     - MIP cuts mcfcut
     - CPX_PARAM_MCFCUTS
   * - :ref:`MIP Cuts - MIP Number of Cut Passes <option-CPLEX-mip_number_of_cut_passes>`
     - MIP limits cutpasses
     - CPX_PARAM_CUTPASS
   * - :ref:`MIP Cuts - Mixed Integer Rounding Cuts <option-CPLEX-mixed_integer_rounding_cuts>`
     - MIP cuts mircut
     - CPX_PARAM_MIRCUTS
   * - :ref:`MIP Cuts - Node Cuts <option-CPLEX-node_cuts>`
     - MIP cuts nodecuts
     - CPX_PARAM_NODECUTS
   * - :ref:`MIP Cuts - RLT Cuts <option-CPLEX-rlt_cuts>`
     - MIP cuts rlt
     - CPX_PARAM_RLTCUTS
   * - :ref:`MIP Cuts - Zero Half Cuts <option-CPLEX-zero_half_cuts>`
     - MIP cuts zerohalf
     - CPX_PARAM_ZEROHALFCUTS
   * - :ref:`MIP Heuristics - Feasibility Pump Heuristic <option-CPLEX-feasibility_pump_heuristic>`
     - MIP strategy fpheur
     - CPX_PARAM_FPHEUR
   * - :ref:`MIP Heuristics - Heuristic Effort <option-CPLEX-heuristic_effort>`
     - MIP strategy heuristiceffort
     - CPX_PARAM_HEUREFFORT
   * - :ref:`MIP Heuristics - Heuristic Frequency <option-CPLEX-heuristic_frequency>`
     - MIP strategy heuristicfreq
     - CPX_PARAM_HEURFREQ
   * - :ref:`MIP Heuristics - Local Branching Heuristic <option-CPLEX-local_branching_heuristic>`
     - MIP strategy lbheur
     - CPX_PARAM_LBHEUR
   * - :ref:`MIP Heuristics - RINS Heuristic Frequency <option-CPLEX-rins_heuristic_frequency>`
     - MIP strategy rinsheur
     - CPX_PARAM_RINSHEUR
   * - :ref:`MIP Preprocessing - Boundstrength <option-CPLEX-boundstrength>`
     - Preprocessing boundstrength
     - CPX_PARAM_BNDSTRENIND
   * - :ref:`MIP Preprocessing - Coefficient Reduction <option-CPLEX-coefficient_reduction>`
     - Preprocessing coeffreduce
     - CPX_PARAM_COEREDIND
   * - :ref:`MIP Preprocessing - Preprocessing Symmetry <option-CPLEX-preprocessing_symmetry>`
     - Preprocessing symmetry
     - CPX_PARAM_SYMMETRY
   * - :ref:`MIP Preprocessing - Presolve Relaxed MIP <option-CPLEX-presolve_relaxed_mip>`
     - Preprocessing relax
     - CPX_PARAM_RELAXPREIND
   * - :ref:`MIP Preprocessing - Repeat Presolve <option-CPLEX-repeat_presolve>`
     - Preprocessing repeatpresolve
     - CPX_PARAM_REPEATPRESOLVE
   * - :ref:`MIP Preprocessing - SOS1 Reformulations <option-CPLEX-sos1_reformulations>`
     - Preprocessing sos1reform
     - CPX_PARAM_SOS1REFORM
   * - :ref:`MIP Preprocessing - SOS2 Reformulations <option-CPLEX-sos2_reformulations>`
     - Preprocessing sos2reform
     - CPX_PARAM_SOS2REFORM
   * - :ref:`MIP Solution Polishing - Polishing Absolute MIP Gap <option-CPLEX-polishing_absolute_mip_gap>`
     - MIP polishafter absmipgap
     - CPX_PARAM_POLISHAFTEREPAGAP
   * - :ref:`MIP Solution Polishing - Polishing Number of Nodes <option-CPLEX-polishing_number_of_nodes>`
     - MIP polishafter nodes
     - CPX_PARAM_POLISHAFTERNODE
   * - :ref:`MIP Solution Polishing - Polishing Number of Solutions <option-CPLEX-polishing_number_of_solutions>`
     - MIP polishafter solutions
     - CPX_PARAM_POLISHAFTERINTSOL
   * - :ref:`MIP Solution Polishing - Polishing Relative MIP Gap <option-CPLEX-polishing_relative_mip_gap>`
     - MIP polishafter mipgap
     - CPX_PARAM_POLISHAFTEREPGAP
   * - :ref:`MIP Solution Polishing - Polishing Time <option-CPLEX-polishing_time>`
     - MIP polishafter time
     - CPX_PARAM_POLISHAFTERTIME
   * - :ref:`MIP Solution Polishing - Polishing Time Deterministic <option-CPLEX-polishing_time_deterministic>`
     - MIP polishafter dettime
     - CPX_PARAM_POLISHAFTERDETTIME
   * - :ref:`MIP Solution Pool - Do Populate <option-CPLEX-do_populate>`
     - 
     - 
   * - :ref:`MIP Solution Pool - Pool Absolute Objective Gap <option-CPLEX-pool_absolute_objective_gap>`
     - MIP pool absgap
     - CPX_PARAM_SOLNPOOLAGAP
   * - :ref:`MIP Solution Pool - Pool Capacity <option-CPLEX-pool_capacity>`
     - MIP pool capacity
     - CPX_PARAM_SOLNPOOLCAPACITY
   * - :ref:`MIP Solution Pool - Pool Intensity <option-CPLEX-pool_intensity>`
     - MIP pool intensity
     - CPX_PARAM_SOLNPOOLINTENSITY
   * - :ref:`MIP Solution Pool - Pool Relative Objective Gap <option-CPLEX-pool_relative_objective_gap>`
     - MIP pool relgap
     - CPX_PARAM_SOLNPOOLGAP
   * - :ref:`MIP Solution Pool - Pool Replacement Strategy <option-CPLEX-pool_replacement_strategy>`
     - MIP pool replace
     - CPX_PARAM_SOLNPOOLREPLACE
   * - :ref:`MIP Solution Pool - Populate Time Limit <option-CPLEX-populate_time_limit>`
     - 
     - 
   * - :ref:`MIP Solution Pool - Population Limit <option-CPLEX-population_limit>`
     - MIP limits populate
     - CPX_PARAM_POPULATELIM
   * - :ref:`Network - Network Extraction Level <option-CPLEX-network_extraction_level>`
     - Network netfind
     - CPX_PARAM_NETFIND
   * - :ref:`Network - Network Feasibility <option-CPLEX-network_feasibility>`
     - Network tolerances feasibility
     - CPX_PARAM_NETEPRHS
   * - :ref:`Network - Network Iterations <option-CPLEX-network_iterations>`
     - Network iterations
     - CPX_PARAM_NETITLIM
   * - :ref:`Network - Network Optimality <option-CPLEX-network_optimality>`
     - Network tolerances optimality
     - CPX_PARAM_NETEPOPT
   * - :ref:`Network - Network Pricing <option-CPLEX-network_pricing>`
     - Network pricing
     - CPX_PARAM_NETPPRIIND
   * - :ref:`Parallel - Auxiliary Root Threads <option-CPLEX-auxiliary_root_threads>`
     - MIP limits auxrootthreads
     - CPX_PARAM_AUXROOTTHREADS
   * - :ref:`Parallel - Global Thread Limit <option-CPLEX-global_thread_limit>`
     - Threads
     - CPX_PARAM_THREADS
   * - :ref:`Parallel - Parallel Mode <option-CPLEX-parallel_mode>`
     - Parallel mode
     - CPX_PARAM_PARALLELMODE
   * - :ref:`Preprocessing - Aggregator <option-CPLEX-aggregator>`
     - Preprocessing aggregator
     - CPX_PARAM_AGGIND
   * - :ref:`Preprocessing - Dependency <option-CPLEX-dependency>`
     - Preprocessing dependency
     - CPX_PARAM_DEPIND
   * - :ref:`Preprocessing - Folding <option-CPLEX-folding>`
     - Preprocessing folding
     - CPX_PARAM_FOLDING
   * - :ref:`Preprocessing - Limit Substitutions <option-CPLEX-limit_substitutions>`
     - Preprocessing fill
     - CPX_PARAM_AGGFILL
   * - :ref:`Preprocessing - Number of Iterations in Presolve <option-CPLEX-number_of_iterations_in_presolve>`
     - Preprocessing numpass
     - CPX_PARAM_PREPASS
   * - :ref:`Preprocessing - Preprocessing Reduction Types <option-CPLEX-preprocessing_reduction_types>`
     - Preprocessing reduce
     - CPX_PARAM_REDUCE
   * - :ref:`Preprocessing - Presolve <option-CPLEX-presolve>`
     - Preprocessing presolve
     - CPX_PARAM_PREIND
   * - :ref:`Preprocessing - Presolve Pass Dual <option-CPLEX-presolve_pass_dual>`
     - Preprocessing dual
     - CPX_PARAM_PREDUAL
   * - :ref:`Preprocessing - Print Presolve Status <option-CPLEX-print_presolve_status>`
     - 
     - 
   * - :ref:`QP - Adjust MIQP <option-CPLEX-adjust_miqp>`
     - Preprocessing qpmakepsd
     - CPX_PARAM_QPMAKEPSDIND
   * - :ref:`QP - Barrier Convergence Tolerance for QCP <option-CPLEX-barrier_convergence_tolerance_for_qcp>`
     - Bar qcpconvergetol
     - CPX_PARAM_BARQCPEPCOMP
   * - :ref:`QP - MIQCP Strategy <option-CPLEX-miqcp_strategy>`
     - MIP strategy miqcpstrat
     - CPX_PARAM_MIQCPSTRAT
   * - :ref:`QP - QCP Dual Values <option-CPLEX-qcp_dual_values>`
     - Preprocessing qcpduals
     - CPX_PARAM_CALCQCPDUALS
   * - :ref:`QP - QP Linearization <option-CPLEX-qp_linearization>`
     - Preprocessing qtolin
     - CPX_PARAM_QTOLININD
   * - :ref:`QP - QP Method <option-CPLEX-qp_method>`
     - Qpmethod
     - CPX_PARAM_QPMETHOD
   * - :ref:`QP - QP Nonzeros Read Limit <option-CPLEX-qp_nonzeros_read_limit>`
     - Read qpnonzeros
     - CPX_PARAM_QPNZREADLIM
   * - :ref:`QP - Solution Target <option-CPLEX-solution_target>`
     - Optimalitytarget
     - CPX_PARAM_OPTIMALITYTARGET
   * - :ref:`Simplex - Crash Ordering <option-CPLEX-crash_ordering>`
     - Simplex crash
     - CPX_PARAM_CRAIND
   * - :ref:`Simplex - Dual Pricing Algorithm <option-CPLEX-dual_pricing_algorithm>`
     - Simplex dgradient
     - CPX_PARAM_DPRIIND
   * - :ref:`Simplex - Dynamic Row Management <option-CPLEX-dynamic_row_management>`
     - simplex dynamicrows
     - CPX_PARAM_DYNAMICROWS
   * - :ref:`Simplex - Feasibility <option-CPLEX-feasibility>`
     - Simplex tolerances feasibility
     - CPX_PARAM_EPRHS
   * - :ref:`Simplex - Markowitz <option-CPLEX-markowitz>`
     - Simplex tolerances markowitz
     - CPX_PARAM_EPMRK
   * - :ref:`Simplex - Optimality <option-CPLEX-optimality>`
     - Simplex tolerances optimality
     - CPX_PARAM_EPOPT
   * - :ref:`Simplex - Perturbation Constant <option-CPLEX-perturbation_constant>`
     - Simplex perturbationlimit
     - CPX_PARAM_EPPER
   * - :ref:`Simplex - Perturbation Indicator <option-CPLEX-perturbation_indicator>`
     - Simplex perturbationlimit
     - CPX_PARAM_PERIND
   * - :ref:`Simplex - Pricing <option-CPLEX-pricing>`
     - Simplex pricing
     - CPX_PARAM_PRICELIM
   * - :ref:`Simplex - Primal Pricing Algorithm <option-CPLEX-primal_pricing_algorithm>`
     - Simplex pgradient
     - CPX_PARAM_PPRIIND
   * - :ref:`Simplex - Refactor <option-CPLEX-refactor>`
     - Simplex refactor
     - CPX_PARAM_REINV
   * - :ref:`Simplex - Sifting From Simplex <option-CPLEX-sifting_from_simplex>`
     - Sifting simplex
     - CPX_PARAM_SIFTSIM
   * - :ref:`Simplex - Singular <option-CPLEX-singular>`
     - Simplex limits singularity
     - CPX_PARAM_SINGLIM
   * - :ref:`Simplex - Stalled Iterations <option-CPLEX-stalled_iterations>`
     - Simplex limits perturbation
     - CPX_PARAM_PERLIM
   * - :ref:`Tuning - Tuning Measure <option-CPLEX-tuning_measure>`
     - Tune measure
     - CPX_PARAM_TUNINGMEASURE
   * - :ref:`Tuning - Tuning Repeater <option-CPLEX-tuning_repeater>`
     - Tune repeat
     - CPX_PARAM_TUNINGREPEAT
   * - :ref:`Tuning - Tuning Time Limit <option-CPLEX-tuning_time_limit>`
     - Tune timelimit
     - CPX_PARAM_TUNINGTILIM
   * - :ref:`Tuning - Tuning Time Limit Deterministic <option-CPLEX-tuning_time_limit_deterministic>`
     - Tune dettimelimit
     - CPX_PARAM_TUNINGDETTILIM


The table below shows Solvers General options that are mapped to CPLEX parameters.

.. list-table::

   * - **Option name in AIMMS**
     - **Name in CPLEX**
     - **Name in CPLEX C API**
   * - :ref:`MIP Options - Cutoff <option-AIMMS-cutoff>`
     - MIP tolerances lowercutoff
     - CPX_PARAM_CUTLO
   * - 
     - MIP tolerances uppercutoff
     - CPX_PARAM_CUTUP
   * - :ref:`MIP Options - Maximal Number of Integer Solutions <option-AIMMS-maximal_number_of_integer_solutions>`
     - MIP limits solutions
     - CPX_PARAM_INTSOLLIM
   * - :ref:`MIP Options - MIP Absolute Optimality Tolerance <option-AIMMS-mip_absolute_optimality_tolerance>`
     - MIP tolerances absmipgap
     - CPX_PARAM_EPAGAP
   * - :ref:`MIP Options - MIP Relative Optimality Tolerance <option-AIMMS-mip_relative_optimality_tolerance>`
     - MIP tolerances mipgap
     - CPX_PARAM_EPGAP
   * - :ref:`Stop Criteria - Iteration Limit <option-AIMMS-iteration_limit>`
     - Simplex limits iterations
     - CPX_PARAM_ITLIM
   * - :ref:`Stop Criteria - Time Limit <option-AIMMS-time_limit>`
     - Timelimit
     - CPX_PARAM_TILIM


