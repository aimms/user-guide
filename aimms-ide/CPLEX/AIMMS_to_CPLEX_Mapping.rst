

.. _AIMMS_to_CPLEX_Mapping:


AIMMS to CPLEX Mapping
===========================

**Description** 

The table below shows in the left column the AIMMS CPLEX options; the middle column displays the CPLEX parameters that are associated with them. The right column displays the constants used in the CPLEX C API.

.. list-table::

   * - **Option name in AIMMS** 
     - **Name in CPLEX** 
     - **Name in CPLEX C API** 
   * - :ref:`option-CPLEX-barrier_algorithm`  
     - Barrier algorithm
     - CPX_PARAM_BARALG
   * - :ref:`option-CPLEX-barrier_always`  
     - 
     - 
   * - :ref:`option-CPLEX-barrier_convergence_tolerance`  
     - Barrier convergetol
     - CPX_PARAM_BAREPCOMP
   * - :ref:`option-CPLEX-barrier_crossover_algorithm` 
     - Barrier crossover
     - CPX_PARAM_BARCROSSALG
   * - :ref:`option-CPLEX-barrier_density_definition`  
     - Barrier colnonzeros
     - CPX_PARAM_BARCOLNZ
   * - :ref:`option-CPLEX-barrier_growth_limit`  
     - Barrier limits growth
     - CPX_PARAM_BARGROWTH
   * - :ref:`option-CPLEX-barrier_iterations`  
     - Barrier limits iteration
     - CPX_PARAM_BARITLIM
   * - :ref:`option-CPLEX-barrier_maximal_number_of_corrections`  
     - Barrier limits corrections
     - CPX_PARAM_BARMAXCOR
   * - :ref:`option-CPLEX-barrier_objective_range`  
     - Barrier limits objrange
     - CPX_PARAM_BAROBJRNG
   * - :ref:`option-CPLEX-barrier_ordering`  
     - Barrier ordering
     - CPX_PARAM_BARORDER
   * - :ref:`option-CPLEX-barrier_progress_solution` 
     - 
     - 
   * - :ref:`option-CPLEX-barrier_start_algorithm`  
     - Barrier startalg	
     - CPX_PARAM_BARSTARTALG
   * - :ref:`option-CPLEX-benders_decomposition_check_limit` 
     - 
     - 
   * - :ref:`option-CPLEX-benders_feasibility_cut_tolerance` 
     - Benders tolerances feasibilitycut
     - CPX_PARAM_BENDERSFEASCUTTOL
   * - :ref:`option-CPLEX-benders_optimality_cut_tolerance` 
     - Benders tolerances optimalitycut
     - CPX_PARAM_BENDERSOPTCUTTOL
   * - :ref:`option-CPLEX-benders_strategy` 
     - Benders strategy
     - CPX_PARAM_BENDERSSTRATEGY
   * - :ref:`option-CPLEX-benders_worker_algorithm` 
     - Benders workeralgorithm
     - CPX_PARAM_WORKERALG
   * - :ref:`option-CPLEX-advanced_start` 
     - Advance
     - CPX_PARAM_ADVIND
   * - :ref:`option-CPLEX-check_solution` 
     - 
     - 
   * - :ref:`option-CPLEX-cleanup_coefficients` 
     - 
     - 
   * - :ref:`option-CPLEX-clock_type` 
     - Clocktype
     - CPX_PARAM_CLOCKTYPE
   * - :ref:`option-CPLEX-cmd_file`  
     - 
     - 
   * - :ref:`option-CPLEX-conflict_algorithm`  
     - Conflict algorithm
     - CPX_PARAM_CONFLICTALG
   * - :ref:`option-CPLEX-data_check_and_modeling_assistance`  
     - Read datacheck
     - CPX_PARAM_DATACHECK
   * - :ref:`option-CPLEX-deterministic_time_limit` 
     - Dettimelimit
     - CPX_PARAM_DETTILIM
   * - :ref:`option-CPLEX-display_solution_statistics`  
     - 
     - 
   * - :ref:`option-CPLEX-farkas_infeasibility_proof`  
     - 
     - 
   * - :ref:`option-CPLEX-feasopt_tolerance` 
     - Feasopt tolerance
     - CPX_PARAM_Feasopt_Tolerance
   * - :ref:`option-CPLEX-lp_file`  
     - 
     - 
   * - :ref:`option-CPLEX-lp_method`  
     - Lpmethod
     - CPX_PARAM_LPMETHOD
   * - :ref:`option-CPLEX-memory_emphasis` 
     - Emphasis memory
     - CPX_PARAM_MEMORYEMPHASIS
   * - :ref:`option-CPLEX-mps`  
     - 
     - 
   * - :ref:`option-CPLEX-numerical_emphasis` 
     - Emphasis numerical
     - CPX_PARAM_NUMERICALEMPHASIS
   * - :ref:`option-CPLEX-ord_file`  
     - 
     - 
   * - :ref:`option-CPLEX-random_seed`  
     - Randomseed
     - CPX_PARAM_RANDOMSEED
   * - :ref:`option-CPLEX-read_parameter_file`  
     - 
     - 
   * - :ref:`option-CPLEX-restart`  
     - 
     - 
   * - :ref:`option-CPLEX-restart_file_number` 
     - 
     - 
   * - :ref:`option-CPLEX-round_coefficients` 
     - 
     - 
   * - :ref:`option-CPLEX-sav_file`  
     - 
     - 
   * - :ref:`option-CPLEX-scale`  
     - Read scale
     - CPX_PARAM_SCAIND
   * - :ref:`option-CPLEX-sensitivity_method`  
     - 
     - 
   * - :ref:`option-CPLEX-sifting_algorithm`  
     - Sifting algorithm
     - CPX_PARAM_SIFTALG
   * - :ref:`option-CPLEX-solution_file`  
     - 
     - 
   * - :ref:`option-CPLEX-solution_type`  
     - Solutiontype
     - CPX_PARAM_SOLUTIONTYPE
   * - :ref:`option-CPLEX-stealth_mode`  
     - 
     - 
   * - :ref:`option-CPLEX-unbounded_ray`  
     - 
     - 
   * - :ref:`option-CPLEX-updates_batch_size`  
     - 
     - 
   * - :ref:`option-CPLEX-write_annotations_file`  
     - 
     - 
   * - :ref:`option-CPLEX-write_parameter_file`  
     - 
     - 
   * - :ref:`option-CPLEX-barrier_display`  
     - Barrier display
     - CPX_PARAM_BARDISPLAY
   * - :ref:`option-CPLEX-clone_log_files` 
     - Output clonelog
     - CPX_PARAM_CLONELOG
   * - :ref:`option-CPLEX-mip_display`  
     - MIP display
     - CPX_PARAM_MIPDISPLAY
   * - :ref:`option-CPLEX-mip_interval` 
     - MIP interval
     - CPX_PARAM_MIPINTERVAL
   * - :ref:`option-CPLEX-multi_objective_display` 
     - Multiobjective display 
     - CPX_PARAM_MULTIOBJDISPLAY
   * - :ref:`option-CPLEX-parameter_display` 
     - Paramdisplay
     - CPX_PARAM_PARAMDISPLAY
   * - :ref:`option-CPLEX-simplex_display`  
     - Simplex display
     - CPX_PARAM_SIMDISPLAY
   * - :ref:`option-CPLEX-tuning_display` 
     - Tune display
     - CPX_PARAM_TUNINGDISPLAY
   * - :ref:`option-CPLEX-backtrack`  
     - MIP strategy backtrack
     - CPX_PARAM_BTTOL
   * - :ref:`option-CPLEX-branch`  
     - MIP strategy branch
     - CPX_PARAM_BRDIR
   * - :ref:`option-CPLEX-difference_objective`  
     - MIP tolerances objdifference
     - CPX_PARAM_OBJDIF
   * - :ref:`option-CPLEX-integrality`  
     - MIP tolerances integrality
     - CPX_PARAM_EPINT
   * - :ref:`option-CPLEX-maximal_number_of_nodes`  
     - MIP limits nodes
     - CPX_PARAM_NODELIM
   * - :ref:`option-CPLEX-mip_basis`  
     - 
     - 
   * - :ref:`option-CPLEX-mip_candidate_list` 
     - MIP limits strongcand
     - CPX_PARAM_STRONGCANDLIM
   * - :ref:`option-CPLEX-mip_dive_strategy`  
     - MIP strategy dive	
     - CPX_PARAM_DIVETYPE
   * - :ref:`option-CPLEX-mip_emphasis` 
     - Emphasis MIP
     - CPX_PARAM_MIPEMPHASIS
   * - :ref:`option-CPLEX-mip_kappa`  
     - MIP strategy kappastats
     - CPX_PARAM_MIPKAPPASTATS
   * - :ref:`option-CPLEX-mip_method`  
     - MIP strategy subalgorithm
     - CPX_PARAM_SUBALG
   * - :ref:`option-CPLEX-mip_priority_order_switch` 
     - MIP strategy order
     - CPX_PARAM_MIPORDIND
   * - :ref:`option-CPLEX-mip_priority_order_type` 
     - MIP ordertype
     - CPX_PARAM_MIPORDTYPE
   * - :ref:`option-CPLEX-mip_probing` 
     - MIP strategy probe
     - CPX_PARAM_PROBE
   * - :ref:`option-CPLEX-mip_search_strategy` 
     - MIP strategy search
     - CPX_PARAM_MIPSEARCH
   * - :ref:`option-CPLEX-mip_start_algorithm`  
     - MIP strategy startalgorithm
     - CPX_PARAM_STARTALG
   * - :ref:`option-CPLEX-mip_tree_memory_limit`  
     - MIP limits treememory
     - CPX_PARAM_TRELIM
   * - :ref:`option-CPLEX-mip_update`  
     - 
     - 
   * - :ref:`option-CPLEX-node_file`  
     - MIP strategy file
     - CPX_PARAM_NODEFILEIND
   * - :ref:`option-CPLEX-mip_node_presolve`  
     - MIP strategy presolvenode
     - CPX_PARAM_PRESLVND
   * - :ref:`option-CPLEX-number_of_repair_attempts` 
     - MIP limits repairtries
     - CPX_PARAM_REPAIRTRIES
   * - :ref:`option-CPLEX-number_of_simplex_iterations` 
     - MIP limits strongit
     - CPX_PARAM_STRONGITLIM
   * - :ref:`option-CPLEX-probing_time`  
     - MIP limits probetime
     - CPX_PARAM_PROBETIME
   * - :ref:`option-CPLEX-probing_time_deterministic`  
     - MIP limits probedettime
     - CPX_PARAM_PROBEDETTIME
   * - :ref:`option-CPLEX-relative_difference_objective`  
     - MIP tolerances relobjdifference
     - CPX_PARAM_RELOBJDIF
   * - :ref:`option-CPLEX-select_variables`  
     - MIP strategy variableselect
     - CPX_PARAM_VARSEL
   * - :ref:`option-CPLEX-selection_of_nodes`  
     - MIP strategy nodeselect
     - CPX_PARAM_NODESEL
   * - :ref:`option-CPLEX-use_generic_callbacks` 
     - 
     - 
   * - :ref:`option-CPLEX-working_memory_limit` 
     - Workmem
     - CPX_PARAM_WORKMEM
   * - :ref:`option-CPLEX-write_mip_starts`  
     - 
     - 
   * - :ref:`option-CPLEX-find_fractional_root_solution` 
     - 
     - 
   * - :ref:`option-CPLEX-lower_objective_stop`  
     - MIP limits lowerobjstop
     - CPX_PARAM_LOWEROBJSTOP
   * - :ref:`option-CPLEX-submip_node_limit` 
     - MIP submip nodelimit
     - CPX_PARAM_SUBMIPNODELIMIT
   * - :ref:`option-CPLEX-submip_scale` 
     - MIP submip scale
     - CPX_PARAM_SUBMIPSCAIND
   * - :ref:`option-CPLEX-submip_start_algorithm` 
     - MIP submip startalg
     - CPX_PARAM_SUBMIPSTARTALG
   * - :ref:`option-CPLEX-submip_subproblem_algorithm` 
     - MIP submip subalg
     - CPX_PARAM_SUBMIPSUBALG
   * - :ref:`option-CPLEX-upper_objective_stop`  
     - MIP limits upperobjstop
     - CPX_PARAM_UPPEROBJSTOP
   * - :ref:`option-CPLEX-write_cuts` 
     - 
     - 
   * - :ref:`option-CPLEX-write_cuts_variable_values` 
     - 
     - 
   * - :ref:`option-CPLEX-bqp_cuts`  
     - MIP cuts bqp
     - CPX_PARAM_BQPCUTS
   * - :ref:`option-CPLEX-clique_cuts`  
     - MIP cuts cliques
     - CPX_PARAM_CLIQUES
   * - :ref:`option-CPLEX-cover_cuts` 
     - MIP cuts covers
     - CPX_PARAM_COVERS
   * - :ref:`option-CPLEX-cut_generation_limit` 
     - MIP limits aggforcut
     - CPX_PARAM_AGGCUTLIM
   * - :ref:`option-CPLEX-cut_limit`  
     - MIP limits eachcutlimit
     - CPX_PARAM_EACHCUTLIM
   * - :ref:`option-CPLEX-cuts_factor`  
     - MIP limits cutsfactor
     - CPX_PARAM_CUTSFACTOR
   * - :ref:`option-CPLEX-disjunctive_cuts` 
     - MIP cuts disjunctive
     - CPX_PARAM_DISJCUTS
   * - :ref:`option-CPLEX-flow_cover_cuts` 
     - MIP cuts flow
     - CPX_PARAM_FLOWCOVERS
   * - :ref:`option-CPLEX-flow_path_cuts` 
     - MIP cuts pathcut
     - CPX_PARAM_FLOWPATHS
   * - :ref:`option-CPLEX-gomory_cuts` 
     - MIP cuts gomory
     - CPX_PARAM_FRACCUTS
   * - :ref:`option-CPLEX-gomory_cuts_candidate_limit` 
     - MIP limits gomorycand
     - CPX_PARAM_FRACCAND
   * - :ref:`option-CPLEX-gomory_cuts_pass_limit` 
     - MIP limits gomorypass
     - CPX_PARAM_FRACPASS
   * - :ref:`option-CPLEX-gub_cover_cuts` 
     - MIP cuts gubcovers
     - CPX_PARAM_GUBCOVERS
   * - :ref:`option-CPLEX-implied_bound_cuts` 
     - MIP cuts implied
     - CPX_PARAM_IMPLBD
   * - :ref:`option-CPLEX-lift_and_project_cuts` 
     - MIP cuts liftproj
     - CPX_PARAM_LANDPCUTS
   * - :ref:`option-CPLEX-local_implied_bound_cuts` 
     - MIP cuts localimplied
     - CPX_PARAM_LOCALIMPLBD
   * - :ref:`option-CPLEX-mcf_cuts`  
     - MIP cuts mcfcut
     - CPX_PARAM_MCFCUTS
   * - :ref:`option-CPLEX-mip_number_of_cut_passes` 
     - MIP limits cutpasses
     - CPX_PARAM_CUTPASS
   * - :ref:`option-CPLEX-mixed_integer_rounding_cuts`  
     - MIP cuts mircut
     - CPX_PARAM_MIRCUTS
   * - :ref:`option-CPLEX-node_cuts`  
     - MIP cuts nodecuts
     - CPX_PARAM_NODECUTS
   * - :ref:`option-CPLEX-rlt_cuts`  
     - MIP cuts rlt
     - CPX_PARAM_RLTCUTS
   * - :ref:`option-CPLEX-zero_half_cuts`  
     - MIP cuts zerohalf
     - CPX_PARAM_ZEROHALFCUTS
   * - :ref:`option-CPLEX-feasibility_pump_heuristic` 
     - MIP strategy fpheur
     - CPX_PARAM_FPHEUR
   * - :ref:`option-CPLEX-heuristic_effort` 
     - MIP strategy heuristiceffort
     - CPX_PARAM_HEUREFFORT
   * - :ref:`option-CPLEX-heuristic_frequency` 
     - MIP strategy heuristicfreq
     - CPX_PARAM_HEURFREQ
   * - :ref:`option-CPLEX-local_branching_heuristic` 
     - MIP strategy lbheur
     - CPX_PARAM_LBHEUR
   * - :ref:`option-CPLEX-rins_heuristic_frequency` 
     - MIP strategy rinsheur
     - CPX_PARAM_RINSHEUR
   * - :ref:`option-CPLEX-boundstrength` 
     - Preprocessing boundstrength
     - CPX_PARAM_BNDSTRENIND
   * - :ref:`option-CPLEX-coefficient_reduction` 
     - Preprocessing coeffreduce
     - CPX_PARAM_COEREDIND
   * - :ref:`option-CPLEX-preprocessing_symmetry`  
     - Preprocessing symmetry
     - CPX_PARAM_SYMMETRY
   * - :ref:`option-CPLEX-presolve_relaxed_mip`  
     - Preprocessing relax
     - CPX_PARAM_RELAXPREIND
   * - :ref:`option-CPLEX-repeat_presolve`  
     - Preprocessing repeatpresolve
     - CPX_PARAM_REPEATPRESOLVE
   * - :ref:`option-CPLEX-sos1_reformulations`  
     - Preprocessing sos1reform
     - CPX_PARAM_SOS1REFORM
   * - :ref:`option-CPLEX-sos2_reformulations`  
     - Preprocessing sos2reform
     - CPX_PARAM_SOS2REFORM
   * - :ref:`option-CPLEX-polishing_absolute_mip_gap`  
     - MIP polishafter absmipgap
     - CPX_PARAM_POLISHAFTEREPAGAP
   * - :ref:`option-CPLEX-polishing_number_of_nodes`  
     - MIP polishafter nodes
     - CPX_PARAM_POLISHAFTERNODE
   * - :ref:`option-CPLEX-polishing_number_of_solutions`  
     - MIP polishafter solutions
     - CPX_PARAM_POLISHAFTERINTSOL
   * - :ref:`option-CPLEX-polishing_relative_mip_gap`  
     - MIP polishafter mipgap
     - CPX_PARAM_POLISHAFTEREPGAP
   * - :ref:`option-CPLEX-polishing_time`  
     - MIP polishafter time
     - CPX_PARAM_POLISHAFTERTIME
   * - :ref:`option-CPLEX-polishing_time_deterministic`  
     - MIP polishafter dettime
     - CPX_PARAM_POLISHAFTERDETTIME
   * - :ref:`option-CPLEX-do_populate`  
     - 
     - 
   * - :ref:`option-CPLEX-pool_absolute_objective_gap` 
     - MIP pool absgap
     - CPX_PARAM_SOLNPOOLAGAP
   * - :ref:`option-CPLEX-pool_capacity`  
     - MIP pool capacity
     - CPX_PARAM_SOLNPOOLCAPACITY
   * - :ref:`option-CPLEX-pool_intensity`  
     - MIP pool intensity
     - CPX_PARAM_SOLNPOOLINTENSITY
   * - :ref:`option-CPLEX-pool_relative_objective_gap` 
     - MIP pool relgap
     - CPX_PARAM_SOLNPOOLGAP
   * - :ref:`option-CPLEX-pool_replacement_strategy`  
     - MIP pool replace
     - CPX_PARAM_SOLNPOOLREPLACE
   * - :ref:`option-CPLEX-populate_time_limit`  
     - 
     - 
   * - :ref:`option-CPLEX-population_limit`  
     - MIP limits populate
     - CPX_PARAM_POPULATELIM
   * - :ref:`option-CPLEX-network_extraction_level` 
     - Network netfind
     - CPX_PARAM_NETFIND
   * - :ref:`option-CPLEX-network_feasibility` 
     - Network tolerances feasibility
     - CPX_PARAM_NETEPRHS
   * - :ref:`option-CPLEX-network_iterations` 
     - Network iterations
     - CPX_PARAM_NETITLIM
   * - :ref:`option-CPLEX-network_optimality` 
     - Network tolerances optimality
     - CPX_PARAM_NETEPOPT
   * - :ref:`option-CPLEX-network_pricing` 
     - Network pricing
     - CPX_PARAM_NETPPRIIND
   * - :ref:`option-CPLEX-auxiliary_root_threads` 
     - MIP limits auxrootthreads
     - CPX_PARAM_AUXROOTTHREADS
   * - :ref:`option-CPLEX-global_thread_limit` 
     - Threads
     - CPX_PARAM_THREADS
   * - :ref:`option-CPLEX-parallel_mode` 
     - Parallel mode
     - CPX_PARAM_PARALLELMODE
   * - :ref:`option-CPLEX-aggregator` 
     - Preprocessing aggregator
     - CPX_PARAM_AGGIND
   * - :ref:`option-CPLEX-dependency` 
     - Preprocessing dependency
     - CPX_PARAM_DEPIND
   * - :ref:`option-CPLEX-folding` 
     - Preprocessing folding
     - CPX_PARAM_FOLDING
   * - :ref:`option-CPLEX-limit_substitutions`  
     - Preprocessing fill
     - CPX_PARAM_AGGFILL
   * - :ref:`option-CPLEX-number_of_iterations_in_presolve` 
     - Preprocessing numpass
     - CPX_PARAM_PREPASS
   * - :ref:`option-CPLEX-preprocessing_reduction_types`  
     - Preprocessing reduce
     - CPX_PARAM_REDUCE
   * - :ref:`option-CPLEX-presolve`  
     - Preprocessing presolve
     - CPX_PARAM_PREIND
   * - :ref:`option-CPLEX-presolve_pass_dual` 
     - Preprocessing dual
     - CPX_PARAM_PREDUAL
   * - :ref:`option-CPLEX-print_presolve_status`  
     - 
     - 
   * - :ref:`option-CPLEX-adjust_miqp`  
     - Preprocessing qpmakepsd
     - CPX_PARAM_QPMAKEPSDIND
   * - :ref:`option-CPLEX-barrier_convergence_tolerance_for_qcp`  
     - Bar qcpconvergetol
     - CPX_PARAM_BARQCPEPCOMP
   * - :ref:`option-CPLEX-miqcp_strategy`  
     - MIP strategy miqcpstrat
     - CPX_PARAM_MIQCPSTRAT
   * - :ref:`option-CPLEX-qcp_dual_values`  
     - Preprocessing qcpduals
     - CPX_PARAM_CALCQCPDUALS
   * - :ref:`option-CPLEX-qp_linearization`  
     - Preprocessing qtolin
     - CPX_PARAM_QTOLININD
   * - :ref:`option-CPLEX-qp_method`  
     - Qpmethod
     - CPX_PARAM_QPMETHOD
   * - :ref:`option-CPLEX-qp_nonzeros_read_limit`  
     - Read qpnonzeros
     - CPX_PARAM_QPNZREADLIM
   * - :ref:`option-CPLEX-solution_target`  
     - Optimalitytarget
     - CPX_PARAM_OPTIMALITYTARGET
   * - :ref:`option-CPLEX-crash_ordering`  
     - Simplex crash
     - CPX_PARAM_CRAIND
   * - :ref:`option-CPLEX-dual_pricing_algorithm`  
     - Simplex dgradient
     - CPX_PARAM_DPRIIND
   * - :ref:`option-CPLEX-dynamic_row_management`  
     - simplex dynamicrows
     - CPX_PARAM_DYNAMICROWS
   * - :ref:`option-CPLEX-feasibility`  
     - Simplex tolerances feasibility
     - CPX_PARAM_EPRHS
   * - :ref:`option-CPLEX-markowitz` 
     - Simplex tolerances markowitz
     - CPX_PARAM_EPMRK
   * - :ref:`option-CPLEX-optimality`  
     - Simplex tolerances optimality
     - CPX_PARAM_EPOPT
   * - :ref:`option-CPLEX-perturbation_constant`  
     - Simplex perturbationlimit
     - CPX_PARAM_EPPER
   * - :ref:`option-CPLEX-perturbation_indicator` 
     - Simplex perturbationlimit
     - CPX_PARAM_PERIND
   * - :ref:`option-CPLEX-pricing`  
     - Simplex pricing
     - CPX_PARAM_PRICELIM
   * - :ref:`option-CPLEX-primal_pricing_algorithm`  
     - Simplex pgradient
     - CPX_PARAM_PPRIIND
   * - :ref:`option-CPLEX-refactor`  
     - Simplex refactor
     - CPX_PARAM_REINV
   * - :ref:`option-CPLEX-sifting_from_simplex` 
     - Sifting simplex
     - CPX_PARAM_SIFTSIM
   * - :ref:`option-CPLEX-singular` 
     - Simplex limits singularity
     - CPX_PARAM_SINGLIM
   * - :ref:`option-CPLEX-stalled_iterations`  
     - Simplex limits perturbation
     - CPX_PARAM_PERLIM
   * - :ref:`option-CPLEX-tuning_measure` 
     - Tune measure
     - CPX_PARAM_TUNINGMEASURE
   * - :ref:`option-CPLEX-tuning_repeater` 
     - Tune repeat
     - CPX_PARAM_TUNINGREPEAT
   * - :ref:`option-CPLEX-tuning_time_limit` 
     - Tune timelimit
     - CPX_PARAM_TUNINGTILIM
   * - :ref:`option-CPLEX-tuning_time_limit_deterministic` 
     - Tune dettimelimit
     - CPX_PARAM_TUNINGDETTILIM


The table below shows Solvers General options that are mapped to CPLEX parameters.

.. list-table::

   * - **Option name in AIMMS** 
     - **Name in CPLEX** 
     - **Name in CPLEX C API** 
   * - :ref:`Options_MIP_Options_-_Cutoff` 
     - MIP tolerances lowercutoff
     - CPX_PARAM_CUTLO
   * - 
     - MIP tolerances uppercutoff
     - CPX_PARAM_CUTUP
   * - :ref:`Options_MIP_Options_-_Maximal_Number_o` 
     - MIP limits solutions
     - CPX_PARAM_INTSOLLIM
   * - :ref:`Options_MIP_Options_-_MIP_Absolute_Opt` 
     - MIP tolerances absmipgap
     - CPX_PARAM_EPAGAP
   * - :ref:`Options_MIP_Options_-_MIP_Relative_Opt` 
     - MIP tolerances mipgap
     - CPX_PARAM_EPGAP
   * - :ref:`Options_Stop_Criteria_-_Iteration_Limi` 
     - Simplex limits iterations
     - CPX_PARAM_ITLIM
   * - :ref:`Options_Stop_Criteria_-_Time_Limit` 
     - Timelimit
     - CPX_PARAM_TILIM

