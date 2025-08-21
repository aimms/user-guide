

.. _CPLEX_to_AIMMS_Mapping:
.. _CPLEX_CPLEX_to_AIMMS_Mapping:


CPLEX to AIMMS Mapping
===========================

**Description** 

The table shows in the left column the parameters from CPLEX that can be set in AIMMS; the right column displays for each CPLEX parameter the associated AIMMS option.

.. list-table::
   :header-rows: 0

   * - **Name in CPLEX**
     - **Option name in AIMMS** 
   * - Advance
     - :ref:`option-CPLEX-advanced_start`
   * - Bar qcpconvergetol
     - :ref:`option-CPLEX-barrier_convergence_tolerance_for_qcp`
   * - Barrier algorithm
     - :ref:`option-CPLEX-barrier_algorithm`
   * - Barrier colnonzeros
     - :ref:`option-CPLEX-barrier_density_definition`
   * - Barrier convergetol
     - :ref:`option-CPLEX-barrier_convergence_tolerance`
   * - Barrier crossover
     - :ref:`option-CPLEX-barrier_crossover_algorithm`
   * - Barrier display
     - :ref:`option-CPLEX-barrier_display`
   * - Barrier limits corrections
     - :ref:`option-CPLEX-barrier_maximal_number_of_corrections`
   * - Barrier limits growth
     - :ref:`option-CPLEX-barrier_growth_limit`
   * - Barrier limits iteration
     - :ref:`option-CPLEX-barrier_iterations`
   * - Barrier limits objrange
     - :ref:`option-CPLEX-barrier_objective_range`
   * - Barrier ordering
     - :ref:`option-CPLEX-barrier_ordering`
   * - Barrier startalg
     - :ref:`option-CPLEX-barrier_start_algorithm`
   * - Benders strategy
     - :ref:`option-CPLEX-benders_strategy`
   * - Benders tolerances feasibilitycut
     - :ref:`option-CPLEX-benders_feasibility_cut_tolerance`
   * - Benders tolerances optimalitycut
     - :ref:`option-CPLEX-benders_optimality_cut_tolerance`
   * - Benders workeralgorithm
     - :ref:`option-CPLEX-benders_worker_algorithm`
   * - Clocktype
     - :ref:`option-CPLEX-clock_type`
   * - Conflict algorithm
     - :ref:`option-CPLEX-conflict_algorithm`
   * - Dettimelimit
     - :ref:`option-CPLEX-deterministic_time_limit`
   * - Emphasis memory
     - :ref:`option-CPLEX-memory_emphasis`
   * - Emphasis MIP
     - :ref:`option-CPLEX-mip_emphasis`
   * - Emphasis numerical
     - :ref:`option-CPLEX-numerical_emphasis`
   * - Feasopt tolerance
     - :ref:`option-CPLEX-feasopt_tolerance`
   * - Lpmethod
     - :ref:`option-CPLEX-lp_method`
   * - MIP cuts bqp
     - :ref:`option-CPLEX-bqp_cuts`
   * - MIP cuts cliques
     - :ref:`option-CPLEX-clique_cuts`
   * - MIP cuts covers
     - :ref:`option-CPLEX-cover_cuts`
   * - MIP cuts disjunctive
     - :ref:`option-CPLEX-disjunctive_cuts`
   * - MIP cuts flow
     - :ref:`option-CPLEX-flow_cover_cuts`
   * - MIP cuts gomory
     - :ref:`option-CPLEX-gomory_cuts`
   * - MIP cuts gubcovers
     - :ref:`option-CPLEX-gub_cover_cuts`
   * - MIP cuts implied
     - :ref:`option-CPLEX-implied_bound_cuts`
   * - MIP cuts liftproj
     - :ref:`option-CPLEX-lift_and_project_cuts`
   * - MIP cuts localimplied
     - :ref:`option-CPLEX-local_implied_bound_cuts`
   * - MIP cuts mcfcut
     - :ref:`option-CPLEX-mcf_cuts`
   * - MIP cuts mircut
     - :ref:`option-CPLEX-mixed_integer_rounding_cuts`
   * - MIP cuts nodecuts
     - :ref:`option-CPLEX-node_cuts`
   * - MIP cuts pathcut
     - :ref:`option-CPLEX-flow_path_cuts`
   * - MIP cuts rlt
     - :ref:`option-CPLEX-rlt_cuts`
   * - MIP cuts zerohalf
     - :ref:`option-CPLEX-zero_half_cuts`
   * - MIP display
     - :ref:`option-CPLEX-mip_display`
   * - MIP interval
     - :ref:`option-CPLEX-mip_interval`
   * - MIP limits aggforcut
     - :ref:`option-CPLEX-cut_generation_limit`
   * - MIP limits auxrootthreads
     - :ref:`option-CPLEX-auxiliary_root_threads`
   * - MIP limits cutpasses
     - :ref:`option-CPLEX-mip_number_of_cut_passes`
   * - MIP limits cutsfactor
     - :ref:`option-CPLEX-cuts_factor`
   * - MIP limits eachcutlimit
     - :ref:`option-CPLEX-cut_limit`
   * - MIP limits gomorycand
     - :ref:`option-CPLEX-gomory_cuts_candidate_limit`
   * - MIP limits gomorypass
     - :ref:`option-CPLEX-gomory_cuts_pass_limit`
   * - MIP limits lowerobjstop
     - :ref:`option-CPLEX-lower_objective_stop`
   * - MIP limits nodes
     - :ref:`option-CPLEX-maximal_number_of_nodes`
   * - MIP limits populate
     - :ref:`option-CPLEX-population_limit`
   * - MIP limits probedettime
     - :ref:`option-CPLEX-probing_time_deterministic`
   * - MIP limits probetime
     - :ref:`option-CPLEX-probing_time`
   * - MIP limits repairtries
     - :ref:`option-CPLEX-number_of_repair_attempts`
   * - MIP limits solutions
     - :ref:`Options_MIP_Options_-_Maximal_Number_o`
   * - MIP limits strongcand
     - :ref:`option-CPLEX-mip_candidate_list`
   * - MIP limits strongit
     - :ref:`option-CPLEX-number_of_simplex_iterations`
   * - MIP limits treememory
     - :ref:`option-CPLEX-mip_tree_memory_limit`
   * - MIP limits upperobjstop
     - :ref:`option-CPLEX-upper_objective_stop`
   * - MIP ordertype
     - :ref:`option-CPLEX-mip_priority_order_type`
   * - MIP polishafter absmipgap
     - :ref:`option-CPLEX-polishing_absolute_mip_gap`
   * - MIP polishafter dettime
     - :ref:`option-CPLEX-polishing_time_deterministic`
   * - MIP polishafter mipgap
     - :ref:`option-CPLEX-polishing_relative_mip_gap`
   * - MIP polishafter nodes
     - :ref:`option-CPLEX-polishing_number_of_nodes`
   * - MIP polishafter solutions
     - :ref:`option-CPLEX-polishing_number_of_solutions`
   * - MIP polishafter time
     - :ref:`option-CPLEX-polishing_time`
   * - MIP pool absgap
     - :ref:`option-CPLEX-pool_absolute_objective_gap`
   * - MIP pool capacity
     - :ref:`option-CPLEX-pool_capacity`
   * - MIP pool intensity
     - :ref:`option-CPLEX-pool_intensity`
   * - MIP pool relgap
     - :ref:`option-CPLEX-pool_relative_objective_gap`
   * - MIP pool replace
     - :ref:`option-CPLEX-pool_replacement_strategy`
   * - MIP strategy backtrack
     - :ref:`option-CPLEX-backtrack`
   * - MIP strategy branch
     - :ref:`option-CPLEX-branch`
   * - MIP strategy dive
     - :ref:`option-CPLEX-mip_dive_strategy`
   * - MIP strategy file
     - :ref:`option-CPLEX-node_file`
   * - MIP strategy fpheur
     - :ref:`option-CPLEX-feasibility_pump_heuristic`
   * - MIP strategy heuristiceffort
     - :ref:`option-CPLEX-heuristic_effort`
   * - MIP strategy heuristicfreq
     - :ref:`option-CPLEX-heuristic_frequency`
   * - MIP strategy kappastats
     - :ref:`option-CPLEX-mip_kappa`
   * - MIP strategy lbheur
     - :ref:`option-CPLEX-local_branching_heuristic`
   * - MIP strategy miqcpstrat
     - :ref:`option-CPLEX-miqcp_strategy`
   * - MIP strategy nodeselect
     - :ref:`option-CPLEX-selection_of_nodes`
   * - MIP strategy order
     - :ref:`option-CPLEX-mip_priority_order_switch`
   * - MIP strategy presolvenode
     - :ref:`option-CPLEX-mip_node_presolve`
   * - MIP strategy probe
     - :ref:`option-CPLEX-mip_probing`
   * - MIP strategy rinsheur
     - :ref:`option-CPLEX-rins_heuristic_frequency`
   * - MIP strategy search
     - :ref:`option-CPLEX-mip_search_strategy`
   * - MIP strategy startalgorithm
     - :ref:`option-CPLEX-mip_start_algorithm`
   * - MIP strategy subalgorithm
     - :ref:`option-CPLEX-mip_method`
   * - MIP strategy variableselect
     - :ref:`option-CPLEX-select_variables`
   * - MIP submip nodelimit
     - :ref:`option-CPLEX-submip_node_limit`
   * - MIP submip scale
     - :ref:`option-CPLEX-submip_scale`
   * - MIP submip startalg
     - :ref:`option-CPLEX-submip_start_algorithm`
   * - MIP submip subalg
     - :ref:`option-CPLEX-submip_subproblem_algorithm`
   * - MIP tolerances absmipgap
     - :ref:`Options_MIP_Options_-_MIP_Absolute_Opt`
   * - MIP tolerances integrality
     - :ref:`option-CPLEX-integrality`
   * - MIP tolerances lowercutoff
     - :ref:`Options_MIP_Options_-_Cutoff`
   * - MIP tolerances mipgap
     - :ref:`Options_MIP_Options_-_MIP_Relative_Opt`
   * - MIP tolerances objdifference
     - :ref:`option-CPLEX-difference_objective`
   * - MIP tolerances relobjdifference
     - :ref:`option-CPLEX-relative_difference_objective`
   * - MIP tolerances uppercutoff
     - :ref:`Options_MIP_Options_-_Cutoff`
   * - Multiobjective display
     - :ref:`option-CPLEX-multi_objective_display`
   * - Network iterations
     - :ref:`option-CPLEX-network_iterations`
   * - Network netfind
     - :ref:`option-CPLEX-network_extraction_level`
   * - Network pricing
     - :ref:`option-CPLEX-network_pricing`
   * - Network tolerances feasibility
     - :ref:`option-CPLEX-network_feasibility`
   * - Network tolerances optimality
     - :ref:`option-CPLEX-network_optimality`
   * - Optimalitytarget
     - :ref:`option-CPLEX-solution_target`
   * - Output clonelog
     - :ref:`option-CPLEX-clone_log_files`
   * - Parallel mode
     - :ref:`option-CPLEX-parallel_mode`
   * - Paramdisplay
     - :ref:`option-CPLEX-parameter_display`
   * - Preprocessing aggregator
     - :ref:`option-CPLEX-aggregator`
   * - Preprocessing boundstrength
     - :ref:`option-CPLEX-boundstrength`
   * - Preprocessing coeffreduce
     - :ref:`option-CPLEX-coefficient_reduction`
   * - Preprocessing dependency
     - :ref:`option-CPLEX-dependency`
   * - Preprocessing dual
     - :ref:`option-CPLEX-presolve_pass_dual`
   * - Preprocessing fill
     - :ref:`option-CPLEX-limit_substitutions`
   * - Preprocessing folding
     - :ref:`option-CPLEX-folding`
   * - Preprocessing numpass
     - :ref:`option-CPLEX-number_of_iterations_in_presolve`
   * - Preprocessing presolve
     - :ref:`option-CPLEX-presolve`
   * - Preprocessing qcpduals
     - :ref:`option-CPLEX-qcp_dual_values`
   * - Preprocessing qpmakepsd
     - :ref:`option-CPLEX-adjust_miqp`
   * - Preprocessing qtolin
     - :ref:`option-CPLEX-qp_linearization`
   * - Preprocessing reduce
     - :ref:`option-CPLEX-preprocessing_reduction_types`
   * - Preprocessing relax
     - :ref:`option-CPLEX-presolve_relaxed_mip`
   * - Preprocessing repeatpresolve
     - :ref:`option-CPLEX-repeat_presolve`
   * - Preprocessing sos1reform
     - :ref:`option-CPLEX-sos1_reformulations`
   * - Preprocessing sos2reform
     - :ref:`option-CPLEX-sos2_reformulations`
   * - Preprocessing symmetry
     - :ref:`option-CPLEX-preprocessing_symmetry`
   * - QPMethod
     - :ref:`option-CPLEX-qp_method`
   * - Randomseed
     - :ref:`option-CPLEX-random_seed`
   * - Read datacheck
     - :ref:`option-CPLEX-data_check_and_modeling_assistance`
   * - Read qpnonzeros
     - :ref:`option-CPLEX-qp_nonzeros_read_limit`
   * - Read scale
     - :ref:`option-CPLEX-scale`
   * - Sifting algorithm
     - :ref:`option-CPLEX-sifting_algorithm`
   * - Sifting simplex
     - :ref:`option-CPLEX-sifting_from_simplex`
   * - Simplex crash
     - :ref:`option-CPLEX-crash_ordering`
   * - Simplex dgradient
     - :ref:`option-CPLEX-dual_pricing_algorithm`
   * - Simplex display
     - :ref:`option-CPLEX-simplex_display`
   * - Simplex dynamicrows
     - :ref:`option-CPLEX-dynamic_row_management`
   * - Simplex limits iterations
     - :ref:`Options_Stop_Criteria_-_Iteration_Limi`
   * - Simplex limits perturbation
     - :ref:`option-CPLEX-stalled_iterations`
   * - Simplex limits singularity
     - :ref:`option-CPLEX-singular`
   * - Simplex perturbationlimit
     - :ref:`option-CPLEX-perturbation_constant`
   * - Simplex perturbationlimit
     - :ref:`option-CPLEX-perturbation_indicator`
   * - Simplex pgradient
     - :ref:`option-CPLEX-primal_pricing_algorithm`
   * - Simplex pricing
     - :ref:`option-CPLEX-pricing`
   * - Simplex refactor
     - :ref:`option-CPLEX-refactor`
   * - Simplex tolerances feasibility
     - :ref:`option-CPLEX-feasibility`
   * - Simplex tolerances markowitz
     - :ref:`option-CPLEX-markowitz`
   * - Simplex tolerances optimality
     - :ref:`option-CPLEX-optimality`
   * - Solutiontype
     - :ref:`option-CPLEX-solution_type`
   * - Threads
     - :ref:`option-CPLEX-global_thread_limit`
   * - Timelimit
     - :ref:`Options_Stop_Criteria_-_Time_Limit`
   * - Tune dettimelimit
     - :ref:`option-CPLEX-tuning_time_limit_deterministic`
   * - Tune display
     - :ref:`option-CPLEX-tuning_display`
   * - Tune measure
     - :ref:`option-CPLEX-tuning_measure`
   * - Tune repeat
     - :ref:`option-CPLEX-tuning_repeater`
   * - Tune timelimit
     - :ref:`option-CPLEX-tuning_time_limit`
   * - Workmem
     - :ref:`option-CPLEX-working_memory_limit`
