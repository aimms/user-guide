

.. _ODH_to_AIMMS_Mapping:


ODH to AIMMS Mapping
========================

**ODH engine parameters** 

The table below shows in the left column the ODH engine parameters from ODH-CPLEX that can be set in AIMMS; the right column displays for each ODH-CPLEX 5.3 parameter the associated AIMMS option.

.. list-table::

   * - **Name in ODH-CPLEX**
     - **Option name in AIMMS**
   * - DECOMPDENSITY
     - :ref:`option-ODHCPLEX-decomposition_density`
   * - DETERMINISTIC
     - :ref:`option-ODHCPLEX-solution_improvement_heuristic_mode`
   * - DIVISOR
     - :ref:`option-ODHCPLEX-initial_divisor_value_sub_models`
   * - FEASOPT
     - :ref:`option-ODHCPLEX-optimization_method`
   * - FEASTOL
     - :ref:`option-ODHCPLEX-odh_feasibility_tolerance`
   * - FIRSTFEAS
     - :ref:`option-ODHCPLEX-first_feasible_heuristic`
   * - FIRSTFEASCONTINUE
     - :ref:`option-ODHCPLEX-first_feasible_heuristic_continue`
   * - FIRSTFEASEFFORT
     - :ref:`option-ODHCPLEX-first_feasible_heuristic_effort_level`
   * - FIRSTFEASSHIFT
     - :ref:`option-ODHCPLEX-first_feasible_heuristic_shift`
   * - GLOBALBOUNDS
     - :ref:`option-ODHCPLEX-global_bounds`
   * - INTERDIV
     - :ref:`option-ODHCPLEX-initial_divisor_value`
   * - MAXBACKTRACK
     - :ref:`option-ODHCPLEX-backtrack_limit`
   * - MAXINFREPEAT
     - :ref:`option-ODHCPLEX-maximum_divisor_repeats_infeasible`
   * - MAXINTERDIV
     - :ref:`option-ODHCPLEX-maximum_divisor_value`
   * - MAXREPEAT
     - :ref:`option-ODHCPLEX-maximum_divisor_repeats`
   * - OBJTARGET
     - :ref:`option-ODHCPLEX-objective_target`
   * - ODHPRESOLVE
     - :ref:`option-ODHCPLEX-odh_presolve`
   * - PENALTY
     - :ref:`option-ODHCPLEX-solution_improvement_heuristic_penalty`
   * - PHASE12
     - :ref:`option-ODHCPLEX-remove_infeasibilities_method`
   * - PRESOLVE
     - :ref:`option-ODHCPLEX-presolve`
   * - PROCESSORLOCK
     - :ref:`option-ODHCPLEX-processor_lock`
   * - QUICKFIRSTSOLVE
     - :ref:`option-ODHCPLEX-quick_first_solve`
   * - RECURSE
     - :ref:`option-ODHCPLEX-recurse`
   * - RECURSEDECOMP
     - :ref:`option-ODHCPLEX-recurse_decomposition_method`
   * - RECURSEITERLIM
     - :ref:`option-ODHCPLEX-recurse_iteration_limit`
   * - RECURSELOG
     - :ref:`option-ODHCPLEX-recurse_log`
   * - RECURSEMINITERLIM
     - :ref:`option-ODHCPLEX-recurse_minimum_iterations`
   * - RECURSESOLITERLIM
     - :ref:`option-ODHCPLEX-recurse_iteration_limit_solution`
   * - REJECTINFSOL
     - :ref:`option-ODHCPLEX-reject_infeasible_solutions`
   * - RELAXSOS2
     - :ref:`option-ODHCPLEX-relax_sos2`
   * - SEED
     - :ref:`option-ODHCPLEX-odh_seed`
   * - STRATEGY
     - :ref:`option-ODHCPLEX-solution_improvement_heuristic_strategy`
   * - SYNCFREQ
     - :ref:`option-ODHCPLEX-thread_synchronization_frequency`
   * - THREADLOG
     - :ref:`option-ODHCPLEX-thread_log`
   * - THREADS
     - :ref:`option-ODHCPLEX-thread_limit`
   * - TIMELIMIT
     - :ref:`Options_Stop_Criteria_-_Time_Limit`
   * - VARIABLECLEAN
     - :ref:`option-ODHCPLEX-clean_variables_sub_models`
   * - WRITESOLUTION
     - :ref:`option-ODHCPLEX-write_solution_file`


**Main CPLEX solve parameters** 

The table below shows CPLEX options for the main CPLEX solve in ODH-CPLEX (if the **Search Mode**  is set to 'Global Solution') or for getting an initial feasible solution (if the **Search Mode**  is set to 'Local Solution'). 
The table below shows in the left column the CPLEX parameters from ODH-CPLEX that can be set in AIMMS; the right column displays for each ODH-CPLEX 5.3 parameter the associated AIMMS option.

.. list-table::

   * - **Name in ODH-CPLEX**
     - **Option name in AIMMS**
   * - CPX_ADVIND
     - :ref:`option-ODHCPLEX-advanced_start`
   * - CPX_AGGCUTLIM
     - :ref:`option-ODHCPLEX-cut_generation_limit`
   * - CPX_AGGFILL
     - :ref:`option-ODHCPLEX-limit_substitutions`
   * - CPX_AGGIND
     - :ref:`option-ODHCPLEX-aggregator`
   * - CPX_AUXROOTTHREADS
     - :ref:`option-ODHCPLEX-auxiliary_root_threads`
   * - CPX_BARALG
     - :ref:`option-ODHCPLEX-barrier_algorithm`
   * - CPX_BARCOLNZ
     - :ref:`option-ODHCPLEX-barrier_density_definition`
   * - CPX_BARCROSSALG
     - :ref:`option-ODHCPLEX-barrier_crossover_algorithm`
   * - CPX_BARDISPLAY
     - :ref:`option-ODHCPLEX-barrier_display`
   * - CPX_BAREPCOMP
     - :ref:`option-ODHCPLEX-barrier_convergence_tolerance`
   * - CPX_BARGROWTH
     - :ref:`option-ODHCPLEX-barrier_growth_limit`
   * - CPX_BARITLIM
     - :ref:`option-ODHCPLEX-barrier_iterations`
   * - CPX_BARMAXCOR
     - :ref:`option-ODHCPLEX-barrier_maximal_number_of_corrections`
   * - CPX_BAROBJRNG
     - :ref:`option-ODHCPLEX-barrier_objective_range`
   * - CPX_BARORDER
     - :ref:`option-ODHCPLEX-barrier_ordering`
   * - CPX_BARQCPEPCOMP
     - :ref:`option-ODHCPLEX-barrier_convergence_tolerance_for_qcp`
   * - CPX_BARSTARTALG
     - :ref:`option-ODHCPLEX-barrier_start_algorithm`
   * - CPX_BNDSTRENIND
     - :ref:`option-ODHCPLEX-boundstrength`
   * - CPX_BQPCUTS
     - :ref:`option-ODHCPLEX-bqp_cuts`
   * - CPX_BRDIR
     - :ref:`option-ODHCPLEX-branch`
   * - CPX_BTTOL
     - :ref:`option-ODHCPLEX-backtrack`
   * - CPX_CLIQUES
     - :ref:`option-ODHCPLEX-clique_cuts`
   * - CPX_CLOCKTYPE
     - :ref:`option-ODHCPLEX-clock_type`
   * - CPX_CLONELOG
     - :ref:`option-ODHCPLEX-clone_log_files`
   * - CPX_COEREDIND
     - :ref:`option-ODHCPLEX-coefficient_reduction`
   * - CPX_CONFLICTALG
     - :ref:`option-ODHCPLEX-conflict_algorithm`
   * - CPX_COVERS
     - :ref:`option-ODHCPLEX-cover_cuts`
   * - CPX_CRAIND
     - :ref:`option-ODHCPLEX-crash_ordering`
   * - CPX_CUTLO
     - :ref:`Options_MIP_Options_-_Cutoff`
   * - CPX_CUTPASS
     - :ref:`option-ODHCPLEX-mip_number_of_cut_passes`
   * - CPX_CUTSFACTOR
     - :ref:`option-ODHCPLEX-cuts_factor`
   * - CPX_CUTUP
     - :ref:`Options_MIP_Options_-_Cutoff`
   * - CPX_DATACHECK
     - :ref:`option-ODHCPLEX-data_check_and_modeling_assistance`
   * - CPX_DEPIND
     - :ref:`option-ODHCPLEX-dependency`
   * - CPX_DETTILIM
     - :ref:`option-ODHCPLEX-deterministic_time_limit`
   * - CPX_DISJCUTS
     - :ref:`option-ODHCPLEX-disjunctive_cuts`
   * - CPX_DIVETYPE
     - :ref:`option-ODHCPLEX-mip_dive_strategy`
   * - CPX_DPRIIND
     - :ref:`option-ODHCPLEX-dual_pricing_algorithm`
   * - CPX_DYNAMICROWS
     - :ref:`option-ODHCPLEX-dynamic_row_management`
   * - CPX_EACHCUTLIM
     - :ref:`option-ODHCPLEX-cut_limit`
   * - CPX_EPAGAP
     - :ref:`Options_MIP_Options_-_MIP_Absolute_Opt`
   * - CPX_EPGAP
     - :ref:`Options_MIP_Options_-_MIP_Relative_Opt`
   * - CPX_EPINT
     - :ref:`option-ODHCPLEX-integrality`
   * - CPX_EPMRK
     - :ref:`option-ODHCPLEX-markowitz`
   * - CPX_EPOPT
     - :ref:`option-ODHCPLEX-optimality`
   * - CPX_EPPER
     - :ref:`option-ODHCPLEX-perturbation_constant`
   * - CPX_EPRHS
     - :ref:`option-ODHCPLEX-feasibility`
   * - CPX_FLOWCOVERS
     - :ref:`option-ODHCPLEX-flow_cover_cuts`
   * - CPX_FLOWPATHS
     - :ref:`option-ODHCPLEX-flow_path_cuts`
   * - CPX_FOLDING
     - :ref:`option-ODHCPLEX-folding`
   * - CPX_FPHEUR
     - :ref:`option-ODHCPLEX-feasibility_pump_heuristic`
   * - CPX_FRACCAND
     - :ref:`option-ODHCPLEX-gomory_cuts_candidate_limit`
   * - CPX_FRACCUTS
     - :ref:`option-ODHCPLEX-gomory_cuts`
   * - CPX_FRACPASS
     - :ref:`option-ODHCPLEX-gomory_cuts_pass_limit`
   * - CPX_GUBCOVERS
     - :ref:`option-ODHCPLEX-gub_cover_cuts`
   * - CPX_HEUREFFORT
     - :ref:`option-ODHCPLEX-heuristic_effort`
   * - CPX_HEURFREQ
     - :ref:`option-ODHCPLEX-heuristic_frequency`
   * - CPX_IMPLBD
     - :ref:`option-ODHCPLEX-implied_bound_cuts`
   * - CPX_INTSOLLIM
     - :ref:`Options_MIP_Options_-_Maximal_Number_o`
   * - CPX_ITLIM
     - :ref:`Options_Stop_Criteria_-_Iteration_Limi`
   * - CPX_LANDPCUTS
     - :ref:`option-ODHCPLEX-lift_and_project_cuts`
   * - CPX_LBHEUR
     - :ref:`option-ODHCPLEX-local_branching_heuristic`
   * - CPX_LOCALIMPLBD
     - :ref:`option-ODHCPLEX-local_implied_bound_cuts`
   * - CPX_MCFCUTS
     - :ref:`option-ODHCPLEX-mcf_cuts`
   * - CPX_MEMORYEMPHASIS
     - :ref:`option-ODHCPLEX-memory_emphasis`
   * - CPX_MIPDISPLAY
     - :ref:`option-ODHCPLEX-mip_display`
   * - CPX_MIPEMPHASIS
     - :ref:`option-ODHCPLEX-mip_emphasis`
   * - CPX_MIPINTERVAL
     - :ref:`option-ODHCPLEX-mip_interval`
   * - CPX_MIPORDIND
     - :ref:`option-ODHCPLEX-mip_priority_order_switch`
   * - CPX_MIPORDTYPE
     - :ref:`option-ODHCPLEX-mip_priority_order_type`
   * - CPX_MIPSEARCH
     - :ref:`option-ODHCPLEX-mip_search_strategy`
   * - CPX_MIQCPSTRAT
     - :ref:`option-ODHCPLEX-miqcp_strategy`
   * - CPX_MIRCUTS
     - :ref:`option-ODHCPLEX-mixed_integer_rounding_cuts`
   * - CPX_NETEPOPT
     - :ref:`option-ODHCPLEX-network_optimality`
   * - CPX_NETEPRHS
     - :ref:`option-ODHCPLEX-network_feasibility`
   * - CPX_NETITLIM
     - :ref:`option-ODHCPLEX-network_iterations`
   * - CPX_NETPPRIIND
     - :ref:`option-ODHCPLEX-network_pricing`
   * - CPX_NODECUTS
     - :ref:`option-ODHCPLEX-node_cuts`
   * - CPX_NODEFILEIND
     - :ref:`option-ODHCPLEX-node_file`
   * - CPX_NODELIM
     - :ref:`option-ODHCPLEX-maximal_number_of_nodes`
   * - CPX_NODESEL
     - :ref:`option-ODHCPLEX-selection_of_nodes`
   * - CPX_NUMERICALEMPHASIS
     - :ref:`option-ODHCPLEX-numerical_emphasis`
   * - CPX_OBJDIF
     - :ref:`option-ODHCPLEX-difference_objective`
   * - CPX_OPTIMALITYTARGET
     - :ref:`option-ODHCPLEX-solution_target`
   * - CPX_PARALLELMODE
     - :ref:`option-ODHCPLEX-parallel_mode`
   * - CPX_PERIND
     - :ref:`option-ODHCPLEX-perturbation_indicator`
   * - CPX_PERLIM
     - :ref:`option-ODHCPLEX-stalled_iterations`
   * - CPX_POLISHAFTERDETTIME
     - :ref:`option-ODHCPLEX-polishing_time_deterministic`
   * - CPX_POLISHAFTEREPAGAP
     - :ref:`option-ODHCPLEX-polishing_absolute_mip_gap`
   * - CPX_POLISHAFTEREPGAP
     - :ref:`option-ODHCPLEX-polishing_relative_mip_gap`
   * - CPX_POLISHAFTERINTSOL
     - :ref:`option-ODHCPLEX-polishing_number_of_solutions`
   * - CPX_POLISHAFTERNODE
     - :ref:`option-ODHCPLEX-polishing_number_of_nodes`
   * - CPX_POLISHAFTERTIME
     - :ref:`option-ODHCPLEX-polishing_time`
   * - CPX_POPULATELIM
     - :ref:`option-ODHCPLEX-population_limit`
   * - CPX_PREDUAL
     - :ref:`option-ODHCPLEX-presolve_pass_dual`
   * - CPX_PREPASS
     - :ref:`option-ODHCPLEX-number_of_iterations_in_presolve`
   * - CPX_PRESLVND
     - :ref:`option-ODHCPLEX-mip_node_presolve`
   * - CPX_PRICELIM
     - :ref:`option-ODHCPLEX-pricing`
   * - CPX_PROBE
     - :ref:`option-ODHCPLEX-mip_probing`
   * - CPX_PROBEDETTIME
     - :ref:`option-ODHCPLEX-probing_time_deterministic`
   * - CPX_PROBETIME
     - :ref:`option-ODHCPLEX-probing_time`
   * - CPX_PPRIIND
     - :ref:`option-ODHCPLEX-primal_pricing_algorithm`
   * - CPX_QPMAKEPSDIND
     - :ref:`option-ODHCPLEX-adjust_miqp`
   * - CPX_QPMETHOD
     - :ref:`option-ODHCPLEX-qp_method`
   * - CPX_QPNZREADLIM
     - :ref:`option-ODHCPLEX-qp_nonzeros_read_limit`
   * - CPX_QTOLININD
     - :ref:`option-ODHCPLEX-qp_linearization`
   * - CPX_RANDOMSEED
     - :ref:`option-ODHCPLEX-random_seed`
   * - CPX_REDUCE
     - :ref:`option-ODHCPLEX-preprocessing_reduction_types`
   * - CPX_REINV
     - :ref:`option-ODHCPLEX-refactor`
   * - CPX_RELAXPREIND
     - :ref:`option-ODHCPLEX-presolve_relaxed_mip`
   * - CPX_RELOBJDIF
     - :ref:`option-ODHCPLEX-relative_difference_objective`
   * - CPX_REPAIRTRIES
     - :ref:`option-ODHCPLEX-number_of_repair_attempts`
   * - CPX_REPEATPRESOLVE
     - :ref:`option-ODHCPLEX-repeat_presolve`
   * - CPX_RINSHEUR
     - :ref:`option-ODHCPLEX-rins_heuristic_frequency`
   * - CPX_RLTCUTS
     - :ref:`option-ODHCPLEX-rlt_cuts`
   * - CPX_SCAIND
     - :ref:`option-ODHCPLEX-scale`
   * - CPX_SIFTALG
     - :ref:`option-ODHCPLEX-sifting_algorithm`
   * - CPX_SIFTSIM
     - :ref:`option-ODHCPLEX-sifting_from_simplex`
   * - CPX_SIMDISPLAY
     - :ref:`option-ODHCPLEX-simplex_display`
   * - CPX_SINGLIM
     - :ref:`option-ODHCPLEX-singular`
   * - CPX_SOLNPOOLAGAP
     - :ref:`option-ODHCPLEX-pool_absolute_objective_gap`
   * - CPX_SOLNPOOLCAPACITY
     - :ref:`option-ODHCPLEX-pool_capacity`
   * - CPX_SOLNPOOLGAP
     - :ref:`option-ODHCPLEX-pool_relative_objective_gap`
   * - CPX_SOLNPOOLINTENSITY
     - :ref:`option-ODHCPLEX-pool_intensity`
   * - CPX_SOLNPOOLREPLACE
     - :ref:`option-ODHCPLEX-pool_replacement_strategy`
   * - CPX_SOS1REFORM
     - :ref:`option-ODHCPLEX-sos1_reformulations`
   * - CPX_SOS2REFORM
     - :ref:`option-ODHCPLEX-sos2_reformulations`
   * - CPX_STARTALG
     - :ref:`option-ODHCPLEX-mip_start_algorithm`
   * - CPX_STRONGCANDLIM
     - :ref:`option-ODHCPLEX-mip_candidate_list`
   * - CPX_STRONGITLIM
     - :ref:`option-ODHCPLEX-number_of_simplex_iterations`
   * - CPX_SUBALG
     - :ref:`option-ODHCPLEX-mip_method`
   * - CPX_SUBMIPNODELIMIT
     - :ref:`option-ODHCPLEX-submip_node_limit`
   * - CPX_SUBMIPSCAIND
     - :ref:`option-ODHCPLEX-submip_scale`
   * - CPX_SUBMIPSTARTALG
     - :ref:`option-ODHCPLEX-submip_start_algorithm`
   * - CPX_SUBMIPSUBALG
     - :ref:`option-ODHCPLEX-submip_subproblem_algorithm`
   * - CPX_SYMMETRY
     - :ref:`option-ODHCPLEX-preprocessing_symmetry`
   * - CPX_THREADS
     - :ref:`option-ODHCPLEX-global_thread_limit`
   * - CPX_TRELIM
     - :ref:`option-ODHCPLEX-mip_tree_memory_limit`
   * - CPX_VARSEL
     - :ref:`option-ODHCPLEX-select_variables`
   * - CPX_WORKMEM
     - :ref:`option-ODHCPLEX-working_memory_limit`
   * - CPX_ZEROHALFCUTS
     - :ref:`option-ODHCPLEX-zero_half_cuts`


**Heuristic sub-model parameters** 

The heuristic sub-model parameters can only be set using a :ref:`ODH-CPLEX_-_Parameter_File`. The syntax for the parameters that influence the heuristic sub-model CPLEX solves is the following: SUB_<parameter> where <parameter> refers to the ODH-CPLEX name in the second table above. The syntax for the parameters that influence the heuristic sub-model CPLEX solves in Phase I is the following: PHASE1_<parameter>.



For example, SUB_CPX_RINSHEUR specifies the RINS heuristic frequency for CPLEX if it used to solve a heuristic sub-model, while PHASE1_CPX_RINSHEUR specifies the RINS heuristic frequency for CPLEX if it used to solve a heuristic sub-model in Phase I.



**Learn more about** 

*	:ref:`ODH-CPLEX_-_Parameter_File` 
*	:ref:`option-ODHCPLEX-search_mode`  
