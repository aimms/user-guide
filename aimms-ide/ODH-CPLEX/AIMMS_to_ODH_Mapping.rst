

.. _AIMMS_to_ODH_Mapping:


AIMMS to ODH Mapping
========================

**ODH engine options** 

The table below shows in the left column the AIMMS options that control the ODH engine; the right column displays for each AIMMS options the associated ODH-CPLEX parameter.

.. list-table::

   * - **Option name in AIMMS** 
     - **Name in ODH-CPLEX** 
   * - :ref:`option-ODHCPLEX-backtrack_limit` 
     - MAXBACKTRACK
   * - :ref:`option-ODHCPLEX-decomposition_density` 
     - DECOMPDENSITY
   * - :ref:`option-ODHCPLEX-global_bounds` 
     - GLOBALBOUNDS
   * - :ref:`option-ODHCPLEX-initial_divisor_value` 
     - INTERDIV
   * - :ref:`option-ODHCPLEX-initial_divisor_value_sub_models` 
     - DIVISOR
   * - :ref:`option-ODHCPLEX-maximum_divisor_repeats` 
     - MAXREPEAT
   * - :ref:`option-ODHCPLEX-maximum_divisor_repeats_infeasible` 
     - MAXINFREPEAT
   * - :ref:`option-ODHCPLEX-maximum_divisor_value` 
     - MAXINTERDIV
   * - :ref:`option-ODHCPLEX-optimization_method` 
     - FEASOPT
   * - :ref:`option-ODHCPLEX-write_decomposition_file` 
     - 
   * - :ref:`option-ODHCPLEX-clean_variables_sub_models` 
     - VARIABLECLEAN
   * - :ref:`option-ODHCPLEX-objective_target` 
     - OBJTARGET
   * - :ref:`option-ODHCPLEX-odh_feasibility_tolerance` 
     - FEASTOL
   * - :ref:`option-ODHCPLEX-odh_presolve` 
     - ODHPRESOLVE
   * - :ref:`option-ODHCPLEX-odh_seed` 
     - SEED
   * - :ref:`option-ODHCPLEX-presolve` 
     - PRESOLVE
   * - :ref:`option-ODHCPLEX-quick_first_solve` 
     - QUICKFIRSTSOLVE
   * - :ref:`option-ODHCPLEX-reject_infeasible_solutions` 
     - REJECTINFSOL
   * - :ref:`option-ODHCPLEX-relax_sos2` 
     - RELAXSOS2
   * - :ref:`option-ODHCPLEX-remove_infeasibilities_method` 
     - PHASE12
   * - :ref:`option-ODHCPLEX-search_mode` 
     - 
   * - :ref:`option-ODHCPLEX-write_solution_file` 
     - WRITESOLUTION
   * - :ref:`option-ODHCPLEX-first_feasible_heuristic` 
     - FIRSTFEAS
   * - :ref:`option-ODHCPLEX-first_feasible_heuristic_continue` 
     - FIRSTFEASCONTINUE
   * - :ref:`option-ODHCPLEX-first_feasible_heuristic_effort_level` 
     - FIRSTFEASEFFORT
   * - :ref:`option-ODHCPLEX-first_feasible_heuristic_shift` 
     - FIRSTFEASSHIFT
   * - :ref:`option-ODHCPLEX-recurse` 
     - RECURSE
   * - :ref:`option-ODHCPLEX-recurse_decomposition_method` 
     - RECURSEDECOMP
   * - :ref:`option-ODHCPLEX-recurse_iteration_limit` 
     - RECURSEITERLIM
   * - :ref:`option-ODHCPLEX-recurse_iteration_limit_solution` 
     - RECURSESOLITERLIM
   * - :ref:`option-ODHCPLEX-recurse_minimum_iterations` 
     - RECURSEMINITERLIM
   * - :ref:`option-ODHCPLEX-solution_improvement_heuristic_mode` 
     - DETERMINISTIC
   * - :ref:`option-ODHCPLEX-solution_improvement_heuristic_penalty` 
     - PENALTY
   * - :ref:`option-ODHCPLEX-solution_improvement_heuristic_strategy` 
     - STRATEGY
   * - :ref:`option-ODHCPLEX-recurse_log` 
     - RECURSELOG
   * - :ref:`option-ODHCPLEX-status_display` 
     - 
   * - :ref:`option-ODHCPLEX-thread_log` 
     - THREADLOG
   * - :ref:`option-ODHCPLEX-thread_limit` 
     - THREADS
   * - :ref:`option-ODHCPLEX-thread_synchronization_frequency` 
     - SYNCFREQ
   * - :ref:`option-ODHCPLEX-processor_lock` 
     - PROCESSORLOCK






**CPLEX solve options** 

The two tables below show options used by ODH-CPLEX for the main CPLEX solve in ODH-CPLEX (if the **Search Mode**  is set to 'Global Solution') or for getting an initial feasible solution (if the **Search Mode**  is set to 'Local Solution').




.. list-table::

   * - **Option name in AIMMS** 
     - **Name in ODH-CPLEX for main CPLEX solve** 
   * - :ref:`option-ODHCPLEX-barrier_algorithm`  
     - CPX_BARALG
   * - :ref:`option-ODHCPLEX-barrier_convergence_tolerance`  
     - CPX_BAREPCOMP
   * - :ref:`option-ODHCPLEX-barrier_crossover_algorithm` 
     - CPX_BARCROSSALG
   * - :ref:`option-ODHCPLEX-barrier_density_definition`  
     - CPX_BARCOLNZ
   * - :ref:`option-ODHCPLEX-barrier_growth_limit`  
     - CPX_BARGROWTH
   * - :ref:`option-ODHCPLEX-barrier_iterations`  
     - CPX_BARITLIM
   * - :ref:`option-ODHCPLEX-barrier_maximal_number_of_corrections`  
     - CPX_BARMAXCOR
   * - :ref:`option-ODHCPLEX-barrier_objective_range`  
     - CPX_BAROBJRNG
   * - :ref:`option-ODHCPLEX-barrier_ordering`  
     - CPX_BARORDER
   * - :ref:`option-ODHCPLEX-barrier_start_algorithm`  
     - CPX_BARSTARTALG
   * - :ref:`option-ODHCPLEX-advanced_start` 
     - CPX_ADVIND
   * - :ref:`option-ODHCPLEX-cleanup_coefficients` 
     - 
   * - :ref:`option-ODHCPLEX-clock_type` 
     - CPX_CLOCKTYPE
   * - :ref:`option-ODHCPLEX-conflict_algorithm`  
     - CPX_CONFLICTALG
   * - :ref:`option-ODHCPLEX-data_check_and_modeling_assistance`  
     - CPX_DATACHECK
   * - :ref:`option-ODHCPLEX-deterministic_time_limit` 
     - CPX_DETTILIM
   * - :ref:`option-ODHCPLEX-lp_file`  
     - 
   * - :ref:`option-ODHCPLEX-memory_emphasis` 
     - CPX_MEMORYEMPHASIS
   * - :ref:`option-ODHCPLEX-mps`  
     - 
   * - :ref:`option-ODHCPLEX-numerical_emphasis` 
     - CPX_NUMERICALEMPHASIS
   * - :ref:`option-ODHCPLEX-ord_file`  
     - 
   * - :ref:`option-ODHCPLEX-random_seed`  
     - CPX_RANDOMSEED
   * - :ref:`option-ODHCPLEX-round_coefficients` 
     - 
   * - :ref:`option-ODHCPLEX-sav_file`  
     - 
   * - :ref:`option-ODHCPLEX-scale`
     - CPX_SCAIND
   * - :ref:`option-ODHCPLEX-sifting_algorithm` 
     - CPX_SIFTALG
   * - :ref:`option-ODHCPLEX-updates_batch_size`  
     - 
   * - :ref:`option-ODHCPLEX-barrier_display`  
     - CPX_BARDISPLAY
   * - :ref:`option-ODHCPLEX-clone_log_files` 
     - CPX_CLONELOG
   * - :ref:`option-ODHCPLEX-mip_display`  
     - CPX_MIPDISPLAY
   * - :ref:`option-ODHCPLEX-mip_interval` 
     - CPX_MIPINTERVAL
   * - :ref:`option-ODHCPLEX-simplex_display`  
     - CPX_SIMDISPLAY
   * - :ref:`option-ODHCPLEX-backtrack`  
     - CPX_BTTOL
   * - :ref:`option-ODHCPLEX-branch`  
     - CPX_BRDIR
   * - :ref:`option-ODHCPLEX-difference_objective`  
     - CPX_OBJDIF
   * - :ref:`option-ODHCPLEX-integrality`  
     - CPX_EPINT
   * - :ref:`option-ODHCPLEX-maximal_number_of_nodes`  
     - CPX_NODELIM
   * - :ref:`option-ODHCPLEX-mip_basis`  
     - 
   * - :ref:`option-ODHCPLEX-mip_candidate_list` 
     - CPX_STRONGCANDLIM
   * - :ref:`option-ODHCPLEX-mip_dive_strategy`  
     - CPX_DIVETYPE
   * - :ref:`option-ODHCPLEX-mip_emphasis` 
     - CPX_MIPEMPHASIS
   * - :ref:`option-ODHCPLEX-mip_method`  
     - CPX_SUBALG
   * - :ref:`option-ODHCPLEX-mip_probing` 
     - CPX_PROBE
   * - :ref:`option-ODHCPLEX-mip_search_strategy` 
     - CPX_MIPSEARCH
   * - :ref:`option-ODHCPLEX-mip_start_algorithm`  
     - CPX_STARTALG
   * - :ref:`option-ODHCPLEX-mip_tree_memory_limit`  
     - CPX_TRELIM
   * - :ref:`option-ODHCPLEX-mip_update`  
     - 
   * - :ref:`option-ODHCPLEX-node_file`  
     - CPX_NODEFILEIND
   * - :ref:`option-ODHCPLEX-mip_node_presolve`  
     - CPX_PRESLVND
   * - :ref:`option-ODHCPLEX-number_of_parallel_threads` 
     - CPX_STRONGTHREADLIM
   * - :ref:`option-ODHCPLEX-number_of_repair_attempts` 
     - CPX_REPAIRTRIES
   * - :ref:`option-ODHCPLEX-number_of_simplex_iterations`
     - CPX_STRONGITLIM
   * - :ref:`option-ODHCPLEX-mip_priority_order_switch`
     - CPX_MIPORDIND
   * - :ref:`option-ODHCPLEX-mip_priority_order_type` 
     - CPX_MIPORDTYPE
   * - :ref:`option-ODHCPLEX-probing_time`  
     - CPX_PROBETIME
   * - :ref:`option-ODHCPLEX-probing_time_deterministic`  
     - CPX_PROBEDETTIME
   * - :ref:`option-ODHCPLEX-relative_difference_objective`  
     - CPX_RELOBJDIF
   * - :ref:`option-ODHCPLEX-select_variables`  
     - CPX_VARSEL
   * - :ref:`option-ODHCPLEX-selection_of_nodes`  
     - CPX_NODESEL
   * - :ref:`option-ODHCPLEX-working_memory_limit`  
     - CPX_WORKMEM
   * - :ref:`option-ODHCPLEX-write_mip_starts`  
     - 
   * - :ref:`option-ODHCPLEX-submip_node_limit` 
     - CPX_SUBMIPNODELIMIT
   * - :ref:`option-ODHCPLEX-submip_scale` 
     - CPX_SUBMIPSCAIND
   * - :ref:`option-ODHCPLEX-submip_start_algorithm` 
     - CPX_SUBMIPSTARTALG
   * - :ref:`option-ODHCPLEX-submip_subproblem_algorithm` 
     - CPX_SUBMIPSUBALG
   * - :ref:`option-ODHCPLEX-bqp_cuts`  
     - CPX_BQPCUTS
   * - :ref:`option-ODHCPLEX-clique_cuts`  
     - CPX_CLIQUES
   * - :ref:`option-ODHCPLEX-cover_cuts` 
     - CPX_COVERS
   * - :ref:`option-ODHCPLEX-cut_generation_limit` 
     - CPX_AGGCUTLIM
   * - :ref:`option-ODHCPLEX-cut_limit`  
     - CPX_EACHCUTLIM
   * - :ref:`option-ODHCPLEX-cuts_factor`  
     - CPX_CUTSFACTOR
   * - :ref:`option-ODHCPLEX-disjunctive_cuts` 
     - CPX_DISJCUTS
   * - :ref:`option-ODHCPLEX-flow_cover_cuts` 
     - CPX_FLOWCOVERS
   * - :ref:`option-ODHCPLEX-flow_path_cuts` 
     - CPX_FLOWPATHS
   * - :ref:`option-ODHCPLEX-gomory_cuts` 
     - CPX_FRACCUTS
   * - :ref:`option-ODHCPLEX-gomory_cuts_candidate_limit` 
     - CPX_FRACCAND
   * - :ref:`option-ODHCPLEX-gomory_cuts_pass_limit` 
     - CPX_FRACPASS
   * - :ref:`option-ODHCPLEX-gub_cover_cuts` 
     - CPX_GUBCOVERS
   * - :ref:`option-ODHCPLEX-implied_bound_cuts` 
     - CPX_IMPLBD
   * - :ref:`option-ODHCPLEX-lift_and_project_cuts` 
     - CPX_LANDPCUTS
   * - :ref:`option-ODHCPLEX-local_implied_bound_cuts` 
     - CPX_LOCALIMPLBD
   * - :ref:`option-ODHCPLEX-mcf_cuts`  
     - CPX_MCFCUTS
   * - :ref:`option-ODHCPLEX-mip_number_of_cut_passes` 
     - CPX_CUTPASS
   * - :ref:`option-ODHCPLEX-mixed_integer_rounding_cuts`  
     - CPX_MIRCUTS
   * - :ref:`option-ODHCPLEX-node_cuts`  
     - CPX_NODECUTS
   * - :ref:`option-ODHCPLEX-rlt_cuts`  
     - CPX_RLTCUTS
   * - :ref:`option-ODHCPLEX-zero_half_cuts`  
     - CPX_ZEROHALFCUTS
   * - :ref:`option-ODHCPLEX-feasibility_pump_heuristic` 
     - CPX_FPHEUR
   * - :ref:`option-ODHCPLEX-heuristic_effort` 
     - CPX_HEUREFFORT
   * - :ref:`option-ODHCPLEX-heuristic_frequency` 
     - CPX_HEURFREQ
   * - :ref:`option-ODHCPLEX-local_branching_heuristic`  
     - CPX_LBHEUR
   * - :ref:`option-ODHCPLEX-rins_heuristic_frequency` 
     - CPX_RINSHEUR
   * - :ref:`option-ODHCPLEX-boundstrength`  
     - CPX_BNDSTRENIND
   * - :ref:`option-ODHCPLEX-coefficient_reduction` 
     - CPX_COEREDIND
   * - :ref:`option-ODHCPLEX-preprocessing_symmetry`  
     - CPX_SYMMETRY
   * - :ref:`option-ODHCPLEX-presolve_relaxed_mip`  
     - CPX_RELAXPREIND
   * - :ref:`option-ODHCPLEX-repeat_presolve`  
     - CPX_REPEATPRESOLVE
   * - :ref:`option-ODHCPLEX-sos1_reformulations` 
     - CPX_SOS1REFORM
   * - :ref:`option-ODHCPLEX-sos2_reformulations` 
     - CPX_SOS2REFORM
   * - :ref:`option-ODHCPLEX-polishing_absolute_mip_gap`  
     - CPX_POLISHAFTEREPAGAP
   * - :ref:`option-ODHCPLEX-polishing_number_of_nodes`  
     - CPX_POLISHAFTERNODE
   * - :ref:`option-ODHCPLEX-polishing_number_of_solutions`  
     - CPX_POLISHAFTERINTSOL
   * - :ref:`option-ODHCPLEX-polishing_relative_mip_gap`  
     - CPX_POLISHAFTEREPGAP
   * - :ref:`option-ODHCPLEX-polishing_time`  
     - CPX_POLISHAFTERTIME
   * - :ref:`option-ODHCPLEX-polishing_time_deterministic`  
     - CPX_POLISHAFTERDETTIME
   * - :ref:`option-ODHCPLEX-do_populate`  
     - 
   * - :ref:`option-ODHCPLEX-pool_absolute_objective_gap` 
     - CPX_SOLNPOOLAGAP
   * - :ref:`option-ODHCPLEX-pool_capacity`  
     - CPX_SOLNPOOLCAPACITY
   * - :ref:`option-ODHCPLEX-pool_intensity`  
     - CPX_SOLNPOOLINTENSITY
   * - :ref:`option-ODHCPLEX-pool_relative_objective_gap` 
     - CPX_SOLNPOOLGAP
   * - :ref:`option-ODHCPLEX-pool_replacement_strategy`  
     - CPX_SOLNPOOLREPLACE
   * - :ref:`option-ODHCPLEX-populate_time_limit`  
     - 
   * - :ref:`option-ODHCPLEX-population_limit`  
     - CPX_POPULATELIM
   * - :ref:`option-ODHCPLEX-network_feasibility` 
     - CPX_NETEPRHS
   * - :ref:`option-ODHCPLEX-network_iterations` 
     - CPX_NETITLIM
   * - :ref:`option-ODHCPLEX-network_optimality` 
     - CPX_NETEPOPT
   * - :ref:`option-ODHCPLEX-network_pricing` 
     - CPX_NETPPRIIND
   * - :ref:`option-ODHCPLEX-auxiliary_root_threads` 
     - CPX_AUXROOTTHREADS
   * - :ref:`option-ODHCPLEX-global_thread_limit` 
     - CPX_THREADS
   * - :ref:`option-ODHCPLEX-parallel_mode` 
     - CPX_PARALLELMODE
   * - :ref:`option-ODHCPLEX-aggregator` 
     - CPX_AGGIND
   * - :ref:`option-ODHCPLEX-dependency`
     - CPX_DEPIND
   * - :ref:`option-ODHCPLEX-folding` 
     - CPX_FOLDING
   * - :ref:`option-ODHCPLEX-limit_substitutions`  
     - CPX_AGGFILL
   * - :ref:`option-ODHCPLEX-number_of_iterations_in_presolve` 
     - CPX_PREPASS
   * - :ref:`option-ODHCPLEX-preprocessing_reduction_types`  
     - CPX_REDUCE
   * - :ref:`option-ODHCPLEX-presolve_pass_dual` 
     - CPX_PREDUAL
   * - :ref:`option-ODHCPLEX-adjust_miqp`  
     - CPX_QPMAKEPSDIND
   * - :ref:`option-ODHCPLEX-barrier_convergence_tolerance_for_qcp`  
     - CPX_BARQCPEPCOMP
   * - :ref:`option-ODHCPLEX-miqcp_strategy`  
     - CPX_MIQCPSTRAT
   * - :ref:`option-ODHCPLEX-qp_linearization`  
     - CPX_QTOLININD
   * - :ref:`option-ODHCPLEX-qp_method`  
     - CPX_QPMETHOD
   * - :ref:`option-ODHCPLEX-qp_nonzeros_read_limit`  
     - CPX_QPNZREADLIM
   * - :ref:`option-ODHCPLEX-solution_target`  
     - CPX_OPTIMALITYTARGET
   * - :ref:`option-ODHCPLEX-crash_ordering`  
     - CPX_CRAIND
   * - :ref:`option-ODHCPLEX-dual_pricing_algorithm`  
     - CPX_DPRIIND
   * - :ref:`option-ODHCPLEX-dynamic_row_management` 
     - CPX_DYNAMICROWS
   * - :ref:`option-ODHCPLEX-feasibility`  
     - CPX_EPRHS
   * - :ref:`option-ODHCPLEX-markowitz` 
     - CPX_EPMRK
   * - :ref:`option-ODHCPLEX-optimality`  
     - CPX_EPOPT
   * - :ref:`option-ODHCPLEX-perturbation_constant`  
     - CPX_EPPER
   * - :ref:`option-ODHCPLEX-perturbation_indicator` 
     - CPX_PERIND
   * - :ref:`option-ODHCPLEX-pricing`  
     - CPX_PRICELIM
   * - :ref:`option-ODHCPLEX-primal_pricing_algorithm`  
     - CPX_PPRIIND
   * - :ref:`option-ODHCPLEX-refactor`  
     - CPX_REINV
   * - :ref:`option-ODHCPLEX-sifting_from_simplex` 
     - CPX_SIFTSIM
   * - :ref:`option-ODHCPLEX-singular` 
     - CPX_SINGLIM
   * - :ref:`option-ODHCPLEX-stalled_iterations`  
     - CPX_PERLIM






The table below shows Solvers General options that are mapped to ODH-CPLEX parameters.




.. list-table::

   * - **Option name in AIMMS** 
     - **Name in ODH-CPLEX** 
   * - :ref:`Options_MIP_Options_-_Cutoff` 
     - CPX_CUTLO
   * - 
     - CPX_CUTUP
   * - :ref:`Options_MIP_Options_-_Maximal_Number_o` 
     - CPX_INTSOLLIM
   * - :ref:`Options_MIP_Options_-_MIP_Absolute_Opt` 
     - CPX_EPAGAP
   * - :ref:`Options_MIP_Options_-_MIP_Relative_Opt` 
     - CPX_EPGAP
   * - :ref:`Options_Stop_Criteria_-_Iteration_Limi` 
     - CPX_ITLIM
   * - :ref:`Options_Stop_Criteria_-_Time_Limit` 
     - TIMELIMIT






**Heuristic sub-model options** 

The heuristic sub-model parameters can only be set using a :ref:`ODH-CPLEX_-_Parameter_File`. The syntax for the parameters that influence the heuristic sub-model CPLEX solves is the following: SUB_<parameter> where <parameter> refers to the ODH-CPLEX name in the second table above. The syntax for the parameters that influence the heuristic sub-model CPLEX solves in Phase I is the following: PHASE1_<parameter>.



For example, SUB_CPX_RINSHEUR specifies the RINS heuristic frequency for CPLEX if it used to solve a heuristic sub-model, while PHASE1_CPX_RINSHEUR specifies the RINS heuristic frequency for CPLEX if it used to solve a heuristic sub-model in Phase I.



**Learn more about** 

*	:ref:`ODH-CPLEX_-_Parameter_File` 
*	:ref:`option-ODHCPLEX-search_mode`  
