

.. _AIMMS_to_KNITRO_Mapping:


AIMMS to Knitro Mapping
============================

**Description** 

The table shows in the left column the AIMMS Knitro options; the right column displays for the AIMMS option the Knitro option that is associated with it.

.. list-table::

   * - **Option name in AIMMS**
     - **Name in Knitro**
   * - :doc:`Advanced - Estimate Noise in the Model <Advanced/KNITRO_Advanced_-_Estimate_Noise_in_the_Model>`
     - findiff_estnoise
   * - :doc:`Advanced - Gradient Computation Method <Advanced/KNITRO_Advanced_-_Gradient_Computation_Method>`
     - gradopt
   * - :doc:`Advanced - Initial Penalty Value <Advanced/KNITRO_Advanced_-_Initial_Penalty_Value>`
     - initpenalty
   * - :doc:`Advanced - Initial Pivot Treshold <Advanced/KNITRO_Advanced_-_Initial_pivot>`
     - linsolver_pivottol
   * - :doc:`Advanced - Initial Trust Scaling Factor <Advanced/KNITRO_Advanced_-_Initial_trust>`
     - delta
   * - :doc:`Advanced - Linesearch Strategy <Advanced/KNITRO_Advanced_-_Linesearch_Strategy>`
     - linesearch
   * - :doc:`Advanced - Linesearch Trials Limit <Advanced/KNITRO_Advanced_-_Linesearch_Trials_Limit>`
     - linesearch_maxtrials
   * - :doc:`Advanced - LP Algorithm <Advanced/KNITRO_Advanced_-_LP_Algorithm>`
     - act_lpalg
   * - :doc:`Advanced - Objective Reduction <Advanced/KNITRO_Advanced_-_Objective_Reduction>`
     - act_lppenalty
   * - :doc:`Advanced - LP Presolve <Advanced/KNITRO_Advanced_-_LP_Presolve>`
     - act_lppresolve
   * - :doc:`Advanced - QP and QCQP Initialization Strategy <Advanced/KNITRO_Advanced_-_QP_and_QCQP_Initialization_Str>`
     - ncvx_qcqp_init
   * - :doc:`Advanced - Solution Progress Iterations <Advanced/KNITRO_Advanced_-_Solution_Progress_Iterations>`
     - xtol_iters
   * - :doc:`Advanced - Solution Progress Tolerance <Advanced/KNITRO_Advanced_-_SolutionProgressTol>`
     - xtol
   * - :doc:`Debugging - Data Check <Debugging/KNITRO_Deb_-_Data_Check>`
     - datacheck
   * - :doc:`Debugging - Debugging MIP output <Debugging/KNITRO_Deb_-_Debugging_MIP_output>`
     - mip_debug
   * - :doc:`Debugging - Debugging Output <Debugging/KNITRO_Deb_-_DebuggingOutput>`
     - debug
   * - :doc:`General - Act QPpenalty <General/KNITRO_General_-_Act_QPpenalty>`
     - act_qppenalty
   * - :doc:`General - Algorithm <General/KNITRO_General_-_Algorithm>`
     - algorithm
   * - :doc:`General - BLAS Option <General/KNITRO_General_-_BLAS_Option>`
     - blasoption
   * - :doc:`General - Honor Bounds <General/KNITRO_General_-_Honor_Bounds>`
     - honorbnds
   * - :doc:`General - Linear Solver <General/KNITRO_General_-_Linear_Solver>`
     - linsolver
   * - :doc:`General - Linear Solver Node Amalgamation <General/KNITRO_General_-_Linear_Solver_Node_Amalgamation>`
     - linsolver_nodeamalg
   * - :doc:`General - Linear Solver Ordering <General/KNITRO_General_-_Linear_Solver_Ordering>`
     - linsolver_ordering
   * - :doc:`General - Linear Solver Out of Core <General/KNITRO_General_-_Linear_Solver_Out_of_Core>`
     - linsolver_ooc
   * - :doc:`General - Linear Solver Scaling <General/KNITRO_General_-_Linear_Solver_Scaling>`
     - linsolver_scaling
   * - :doc:`General - Linear System Max Iterative Refinements <General/KNITRO_General_-_Linear_System_Max_Iterative_Re>`
     - linsolver_maxitref
   * - :doc:`General - LP Solver <General/KNITRO_General_-_LP_Solver>`
     - act_lpsolver
   * - :doc:`General - Mark as Convex <General/KNITRO_General_-_Mark_as_Convex>`
     - convex
   * - :doc:`General - QP Algorithm <General/KNITRO_General_-_QP_Algorithm>`
     - act_qpalg
   * - :doc:`General - Restarts <General/KNITRO_General_-_Restarts>`
     - restarts
   * - :doc:`General - Restarts Iteration Limit <General/KNITRO_General_-_Restarts_Iteration_Limit>`
     - restarts_maxit
   * - :doc:`General - Scale Variables <General/KNITRO_General_-_Scale_Variables>`
     - scale_vars
   * - :doc:`General - Scaling <General/KNITRO_General_-_Scaling>`
     - scale
   * - :doc:`General - Unboundedness Range <General/KNITRO_General_-_Unbound_range>`
     - objrange
   * - :doc:`General - Warm Start Strategy <General/KNITRO_General_-_Warm_Start_Strategy>`
     - strat_warm_start
   * - :doc:`Hessian - Hessian Computation Method <Hessian/KNITRO_Hessian_-_Hes_Comp_Meth>`
     - hessopt
   * - :doc:`Hessian - Limited Memory Size <Hessian/KNITRO_Hessian_-_Limited_Memory_Size>`
     - lmsize
   * - :doc:`Hessian - Second Order Correction <Hessian/KNITRO_Hessian_-_SecondOrderCor>`
     - soc
   * - :doc:`Interior Point - Barrier Corrector Steps Limit <Interior Point/KNITRO_IP_-_Barrier_Corrector_Steps_Limit>`
     - bar_maxcorrectors
   * - :doc:`Interior Point - Barrier Enable Conic <Interior Point/KNITRO_IP_-_Barrier_Enable_Conic>`
     - bar_conic_enable
   * - :doc:`Interior Point - Barrier Globalize <Interior Point/KNITRO_IP_-_Barrier_Globalize>`
     - bar_globalize
   * - :doc:`Interior Point - Barrier Maximum Mu <Interior Point/KNITRO_IP_-_Barrier_Maximum_Mu>`
     - bar_maxmu
   * - :doc:`Interior Point - Barrier MPEC Heuristic <Interior Point/KNITRO_IP_-_Barrier_MPEC_Heuristic>`
     - bar_mpec_heuristic
   * - :doc:`Interior Point - Barrier Parameter Strategy <Interior Point/KNITRO_IP_-_Bar_Par_Strategy>`
     - bar_murule
   * - :doc:`Interior Point - Barrier Penalty Constraint Strategy <Interior Point/KNITRO_IP_-_Barrier_Penalty_Constraint_St>`
     - bar_penaltycons
   * - :doc:`Interior Point - Barrier Penalty Parameter Strategy <Interior Point/KNITRO_IP_-_Barrier_Penalty_Parameter_St>`
     - bar_penaltyrule
   * - :doc:`Interior Point - Barrier Refinement <Interior Point/KNITRO_IP_-_Barrier_Refinement>`
     - bar_refinement
   * - :doc:`Interior Point - Barrier Relax Constraints <Interior Point/KNITRO_IP_-_Barrier_Relax_Constraints>`
     - bar_relaxcons
   * - :doc:`Interior Point - Barrier Slack Bound Push <Interior Point/KNITRO_IP_-_Barrier_Slack_Bound_Push>`
     - bar_slackboundpush
   * - :doc:`Interior Point - Barrier Switch Objective <Interior Point/KNITRO_IP_-_Barrier_Switch_Objective>`
     - bar_switchobj
   * - :doc:`Interior Point - Barrier Switch Rule <Interior Point/KNITRO_IP_-_Barrier_Switch_Rule>`
     - bar_switchrule
   * - :doc:`Interior Point - Barrier Watchdog <Interior Point/KNITRO_IP_-_Barrier_Watchdog>`
     - bar_watchdog
   * - :doc:`Interior Point - Conjugate Gradient Iteration Limit <Interior Point/KNITRO_IP_-_ConjugateGradIter>`
     - cg_maxit
   * - :doc:`Interior Point - Conjugate Gradient Memory Limit <Interior Point/KNITRO_IP_-_Conjugate_Gradient_Memory_Limit>`
     - cg_pmem
   * - :doc:`Interior Point - Conjugate Gradient Preconditioner <Interior Point/KNITRO_IP_-_Conjugate_Gradient_Preconditio>`
     - cg_precond
   * - :doc:`Interior Point - Conjugate Gradient Stopping Tolerance <Interior Point/KNITRO_IP_-_Conjugate_Gradient_Stopping_To>`
     - cg_stoptol
   * - :doc:`Interior Point - Crossover Iterations Limit <Interior Point/KNITRO_IP_-_CrossoverIterLimit>`
     - bar_maxcrossit
   * - :doc:`Interior Point - Direct Step Interval <Interior Point/KNITRO_IP_-_Direct_Step_Interval>`
     - bar_directinterval
   * - :doc:`Interior Point - Feasible Mode <Interior Point/KNITRO_IP_-_Feasible_mode>`
     - bar_feasible
   * - :doc:`Interior Point - Feasible Mode Activation Tolerance <Interior Point/KNITRO_IP_-_Feas_mode_act_tol>`
     - bar_feasmodetol
   * - :doc:`Interior Point - Initial Barrier Parameter Value <Interior Point/KNITRO_IP_-_InitBarParValue>`
     - bar_initmu
   * - :doc:`Interior Point - Initial Barrier Penalty Value MPEC <Interior Point/KNITRO_IP_-_Initial_Barrier_Penalty_Value>`
     - bar_initpi_mpec
   * - :doc:`Interior Point - Initial Point Strategy <Interior Point/KNITRO_IP_-_Initial_Point_Strat>`
     - bar_initpt
   * - :doc:`Interior Point - Linear System Form Used <Interior Point/KNITRO_IP_-_Linear_System_Form_Used>`
     - bar_linsys
   * - :doc:`Interior Point - Linear System Memory Usage <Interior Point/KNITRO_IP_-_Linear_System_Memory_Usage>`
     - bar_linsys_storage
   * - :doc:`Interior Point - Refactorization Limit <Interior Point/KNITRO_IP_-_RefactorizationLim>`
     - bar_maxrefactor
   * - :doc:`MIP - Integrality <MIP/KNITRO_MIP_-_Integrality>`
     - mip_integer_tol
   * - :doc:`MIP - Maximal Number of Nodes <MIP/KNITRO_MIP_-_Maximal_Number_of_Nodes>`
     - mip_maxnodes
   * - :doc:`MIP - Maximal Number of Subproblem Solves <MIP/KNITRO_MIP_-_Maximal_Nr_Subproblem_Slvs>`
     - mip_maxsolves
   * - :doc:`MIP - MIP Algorithm <MIP/KNITRO_MIP_-_MIP_Algorithm>`
     - mip_lpalg
   * - :doc:`MIP - MIP Branching Rule <MIP/KNITRO_MIP_-_MIP_Branching_Rule>`
     - mip_branchrule
   * - :doc:`MIP - MIP GUB Branch <MIP/KNITRO_MIP_-_MIP_GUB_Branch>`
     - mip_gub_branch
   * - :doc:`MIP - MIP Heuristic <MIP/KNITRO_MIP_-_MIP_Heuristic>`
     - mip_heuristic
   * - :doc:`MIP - MIP Heuristic Diving <MIP/KNITRO_MIP_-_MIP_Heuristic_Diving>`
     - mip_heuristic_diving
   * - :doc:`MIP - MIP Heuristic Feasibility Pump <MIP/KNITRO_MIP_-_MIP_Heuristic_Feasibility_Pump>`
     - mip_heuristic_feaspump
   * - :doc:`MIP - MIP Heuristic Iteration Limit <MIP/KNITRO_MIP_-_MIP_Heuristic_Iteration_Limit>`
     - mip_heuristic_maxit
   * - :doc:`MIP - MIP Heuristic Large Neighborhood Search <MIP/KNITRO_MIP_-_MIP_Heuristic_Large_Neighborhood_Search>`
     - mip_heuristic_lns
   * - :doc:`MIP - MIP Heuristic Local Search <MIP/KNITRO_MIP_-_MIP_Heuristic_Local_Search>`
     - mip_heuristic_local_search
   * - :doc:`MIP - MIP Heuristic MPEC <MIP/KNITRO_MIP_-_MIP_Heuristic_MPEC>`
     - mip_heuristic_mpec
   * - :doc:`MIP - MIP Heuristic Strategy <MIP/KNITRO_MIP_-_MIP_Heuristic_Strategy>`
     - mip_heuristic_strategy
   * - :doc:`MIP - MIP Heuristic Terminate <MIP/KNITRO_MIP_-_MIP_Heuristic_Terminate>`
     - mip_heuristic_terminate
   * - :doc:`MIP - MIP Implications <MIP/KNITRO_MIP_-_MIP_Implications>`
     - mip_implications
   * - :doc:`MIP - MIP Integer Variables Relaxable <MIP/KNITRO_MIP_-_MIP_Integer_Variables_Relaxabl>`
     - mip_relaxable
   * - :doc:`MIP - MIP Integer Variables Strategy <MIP/KNITRO_MIP_-_MIP_Integer_Variables_Strategy>`
     - mip_intvar_strategy
   * - :doc:`MIP - MIP Method <MIP/KNITRO_MIP_-_MIP_Method>`
     - mip_method
   * - :doc:`MIP - MIP MISQP Heuristic <MIP/KNITRO_MIP_-_MIP_MISQP_Heuristic>`
     - mip_heuristic_misqp
   * - :doc:`MIP - MIP Multistart <MIP/KNITRO_MIP_-_MIP_Multistart>`
     - mip_multistart
   * - :doc:`MIP - MIP Objective Cutoff Value <MIP/KNITRO_MIP_-_MIP_Objective_Cutoff_Value>`
     - mip_cutoff
   * - :doc:`MIP - MIP Pseudo Cost Initialization <MIP/KNITRO_MIP_-_MIP_Pseudo_Cost_Initialization>`
     - mip_pseudoinit
   * - :doc:`MIP - MIP Restart <MIP/KNITRO_MIP_-_MIP_Restart>`
     - mip_restart
   * - :doc:`MIP - MIP Rounding <MIP/KNITRO_MIP_-_MIP_Rounding>`
     - mip_rounding
   * - :doc:`MIP - MIP Start Algorithm <MIP/KNITRO_MIP_-_MIP_Start_Algorithm>`
     - mip_rootalg
   * - :doc:`MIP - MIP Terminate <MIP/KNITRO_MIP_-_MIP_Terminate>`
     - mip_terminate
   * - :doc:`MIP - Node Algorithm <MIP/KNITRO_MIP_-_Node_Algorithm>`
     - mip_nodealg
   * - :doc:`MIP - Node Selection <MIP/KNITRO_MIP_-_Node_Selection>`
     - mip_selectrule
   * - :doc:`MIP - Node Selection_Direction <MIP/KNITRO_MIP_-_Node_Selection_Direction>`
     - mip_selectdir
   * - :doc:`MIP - Strong Branching Candidates Limit <MIP/KNITRO_MIP_-_Strong_Branch_Candidates_Limit>`
     - mip_strong_candlim
   * - :doc:`MIP - Strong Branching Iteration Limit <MIP/KNITRO_MIP_-_Strong_Branch_Iter_Limit>`
     - mip_strong_maxit
   * - :doc:`MIP - Strong Branching Level <MIP/KNITRO_MIP_-_Strong_Branching_Level>`
     - mip_strong_level
   * - :doc:`MIP Cuts - Clique Cuts <MIP Cuts/KNITRO_MIP_Cuts_-_Clique_cuts>`
     - mip_clique
   * - :doc:`MIP Cuts - Flow Cover Cuts <MIP Cuts/KNITRO_MIP_Cuts_-_Flowcover_Cuts>`
     - mip_cut_flowcover
   * - :doc:`MIP Cuts - Gomory Cuts <MIP Cuts/KNITRO_MIP_Cuts_-_Gomory_Cuts>`
     - mip_gomory
   * - :doc:`MIP Cuts - Knapsack Cuts <MIP Cuts/KNITRO_MIP_Cuts_-_Knapsack_cuts>`
     - mip_knapsack
   * - :doc:`MIP Cuts - Lift and Project Cuts <MIP Cuts/KNITRO_MIP_Cuts_-_Lift_and_Project_Cuts>`
     - mip_liftproject
   * - :doc:`MIP Cuts - MIR Cuts <MIP Cuts/KNITRO_MIP_Cuts_-_MIR_cuts>`
     - mip_mir
   * - :doc:`MIP Cuts - Probing Cuts <MIP Cuts/KNITRO_MIP_Cuts_-_Probing_Cuts>`
     - mip_cut_probing
   * - :doc:`MIP Cuts - Zero Half Cuts <MIP Cuts/KNITRO_MIP_Cuts_-_Zero_Half_cuts>`
     - mip_zerohalf
   * - :doc:`Multistart - Multistart <Multistart/KNITRO_MS_-_Multistart>`
     - ms_enable
   * - :doc:`Multistart - Multistart Deterministic <Multistart/KNITRO_MS_-_Multistart_Deterministic>`
     - ms_deterministic
   * - :doc:`Multistart - Multistart Initial Points Cluster <Multistart/KNITRO_MS_-_Multistart_Initial_Points_Clus>`
     - ms_initpt_cluster
   * - :doc:`Multistart - Multistart Range <Multistart/KNITRO_MS_-_Multistart_Range>`
     - ms_startptrange
   * - :doc:`Multistart - Multistart Range Unbounded Variable <Multistart/KNITRO_MS_-_Multistart_Range_Unbounded_Var>`
     - ms_maxbndrange
   * - :doc:`Multistart - Multistart Seed <Multistart/KNITRO_MS_-_Multistart_Seed>`
     - ms_seed
   * - :doc:`Multistart - Multistart Termination Condition <Multistart/KNITRO_MS_-_MS_Termination_Conditi>`
     - ms_terminate
   * - :doc:`Multistart - Number of Best Solutions <Multistart/KNITRO_MS_-_Number_of_Best_Solutions>`
     - ms_num_to_save
   * - :doc:`Multistart - Number of Multistart Points <Multistart/KNITRO_MS_-_Nr_multi_points>`
     - ms_maxsolves
   * - :doc:`Multistart - Solution Distance <Multistart/KNITRO_MS_-_Solution_Distance>`
     - ms_savetol
   * - :doc:`Parallel - Number of Gradient Computation Threads <Parallel/KNITRO_Par_-_Number_of_Gradient_Computation_Threads>`
     - findiff_numthreads
   * - :doc:`Parallel - Number of BLAS Threads <Parallel/KNITRO_Par_-_Number_of_BLAS_threads>`
     - blas_numthreads
   * - :doc:`Parallel - Number of Linear System Threads <Parallel/KNITRO_Par_-_Number_of_Lin_Sys_Threads>`
     - linsolver_numthreads
   * - :doc:`Parallel - Number of MIP Threads <Parallel/KNITRO_Par_-_Number_of_MIP_Threads>`
     - mip_numthreads
   * - :doc:`Parallel - Number of Multistart Threads <Parallel/KNITRO_Par_-_Number_of_Multistart_Threads>`
     - ms_numthreads
   * - :doc:`Parallel - Number of Threads <Parallel/KNITRO_Par_-_Number_of_Threads>`
     - numthreads
   * - :doc:`Presolve - Presolve <Presolve/KNITRO_Presolve_-_Presolve>`
     - presolve
   * - :doc:`Presolve - Presolve Initial Point <Presolve/KNITRO_Presolve_-_Presolve_Initial_Point_Shift>`
     - presolve_initpt
   * - :doc:`Presolve - Presolve Level <Presolve/KNITRO_Presolve_-_Presolve_Level>`
     - presolve_level
   * - :doc:`Presolve - Presolve Passes <Presolve/KNITRO_Presolve_-_Presolve_Passes>`
     - presolve_passes
   * - :doc:`Presolve - Presolve Redundant Constraints <Presolve/KNITRO_Presolve_-_Presolve_Redundant_Constraints>`
     - presolveop_redundant
   * - :doc:`Presolve - Presolve Substitution <Presolve/KNITRO_Presolve_-_Presolve_Substitution>`
     - presolveop_substitution
   * - :doc:`Presolve - Presolve Substitution Tolerance <Presolve/KNITRO_Presolve_-_Presolve_Substitution_Tolerance>`
     - presolveop_substitution_tol
   * - :doc:`Presolve - Presolve Tolerance <Presolve/KNITRO_Presolve_-_Presolve_Tolerance>`
     - presolve_tol
   * - :doc:`Presolve - Tighten Variable Bounds <Presolve/KNITRO_Presolve_-_Tighten_Variable_Bounds>`
     - presolveop_tighten
   * - :doc:`Reporting - MIP Output Level <Reporting/KNITRO_Reporting_-_MIP_Output_Level>`
     - mip_outinterval
   * - :doc:`Reporting - Multi Algorithm Output <Reporting/KNITRO_Reporting_-_Multi_Algorithm_Output>`
     - ma_outsub
   * - :doc:`Reporting - Status File Display <Reporting/KNITRO_Reporting_-_StatusFileDi>`
     - outlev
   * - :doc:`Termination - Absolute Optimality Tolerance <Termination/KNITRO_Term_-_AbsOptTol>`
     - opttol_abs
   * - :doc:`Termination - Function Evaluations Limit <Termination/KNITRO_Term_-_Function_Evaluations_Limit>`
     - maxfevals
   * - :doc:`Termination - Infeasibility Tolerance Iteration Limit <Termination/KNITRO_Term_-_Infeas_Tol_Iteration_Limit>`
     - infeastol_iters
   * - :doc:`Termination - Multi Algorithm Termination <Termination/KNITRO_Term_-_Multi_Algorithm_Termination>`
     - ma_terminate
   * - :doc:`Termination - Objective Goal <Termination/KNITRO_Term_-_Objective_Goal>`
     - fstopval
   * - :doc:`Termination - Relative Improvement Iterations <Termination/KNITRO_Term_-_Relative_Improvement_Iterations>`
     - ftol_iters
   * - :doc:`Termination - Relative Improvement Tolerance <Termination/KNITRO_Term_-_Relative_Improvement_Tolerance>`
     - ftol
   * - :doc:`Termination - Relative Optimality Tolerance <Termination/KNITRO_Term_-_RelOptTol>`
     - opttol
   * - :doc:`Tolerances - Absolute Feasibility Tolerance <Tolerances/KNITRO_Tol_-_AbsFeasTol>`
     - feastol_abs
   * - :doc:`Tolerances - Infeasibility Tolerance <Tolerances/KNITRO_Tol_-_Infeasibility_Tolerance>`
     - infeastol
   * - :doc:`Tolerances - LP Feasibility Tolerance <Tolerances/KNITRO_Tol_-_LP_Feasibility_Tolerance>`
     - act_lpfeastol
   * - :doc:`Tolerances - Relative Feasibility Tolerance <Tolerances/KNITRO_Tol_-_RelFeasTol>`
     - feastol
   * - :doc:`Tuner - Tuner <Tuner/KNITRO_Tuner_-_Tuner>`
     - tuner
   * - :doc:`Tuner - Tuner Output <Tuner/KNITRO_Tuner_-_Tuner_Output>`
     - tuner_outsub
   * - :doc:`Tuner - Tuner Terminate <Tuner/KNITRO_Tuner_-_Tuner_Terminate>`
     - tuner_terminate
   * - :doc:`Tuner - Tuner Time Limit <Tuner/KNITRO_Tuner_-_Tuner_Time_Limit>`
     - tuner_maxtime_cpu
