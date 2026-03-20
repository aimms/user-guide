

.. _KNITRO_to_AIMMS_Mapping:


Knitro to AIMMS Mapping
============================

**Description** 

The table shows in the left column the parameters from Knitro that can be set in AIMMS; the right column displays for each Knitro option the associated AIMMS option.
	
.. list-table::

   * - **Name in Knitro**
     - **Option name in AIMMS**
   * - act_lpalg
     - :doc:`Advanced - LP Algorithm <Advanced/KNITRO_Advanced_-_LP_Algorithm>`
   * - act_lpfeastol
     - :doc:`Tolerances - LP Feasibility Tolerance <Tolerances/KNITRO_Tol_-_LP_Feasibility_Tolerance>`
   * - act_lppenalty
     - :doc:`Advanced - Objective Reduction <Advanced/KNITRO_Advanced_-_Objective_Reduction>`
   * - act_lppresolve
     - :doc:`Advanced - LP Presolve <Advanced/KNITRO_Advanced_-_LP_Presolve>`
   * - act_lpsolver
     - :doc:`General - LP Solver <General/KNITRO_General_-_LP_Solver>`
   * - act_qpalg
     - :doc:`General - QP Algorithm <General/KNITRO_General_-_QP_Algorithm>`
   * - act_qppenalty
     - :doc:`General - Act QPpenalty <General/KNITRO_General_-_Act_QPpenalty>`
   * - bar_conic_enable
     - :doc:`Interior Point - Barrier Enable Conic <Interior Point/KNITRO_IP_-_Barrier_Enable_Conic>`
   * - bar_directinterval
     - :doc:`Interior Point - Direct Step Interval <Interior Point/KNITRO_IP_-_Direct_Step_Interval>`
   * - bar_feasible
     - :doc:`Interior Point - Feasible Mode <Interior Point/KNITRO_IP_-_Feasible_mode>`
   * - bar_feasmodetol
     - :doc:`Interior Point - Feasible Mode Activation Tolerance <Interior Point/KNITRO_IP_-_Feas_mode_act_tol>`
   * - bar_globalize
     - :doc:`Interior Point - Barrier Globalize <Interior Point/KNITRO_IP_-_Barrier_Globalize>`
   * - bar_initmu
     - :doc:`Interior Point - Initial Barrier Parameter Value <Interior Point/KNITRO_IP_-_InitBarParValue>`
   * - bar_initpi_mpec
     - :doc:`Interior Point - Initial Barrier Penalty Value MPEC <Interior Point/KNITRO_IP_-_Initial_Barrier_Penalty_Value>`
   * - bar_initpt
     - :doc:`Interior Point - Initial Point Strategy <Interior Point/KNITRO_IP_-_Initial_Point_Strat>`
   * - bar_linsys
     - :doc:`Interior Point - Linear System Form Used <Interior Point/KNITRO_IP_-_Linear_System_Form_Used>`
   * - bar_linsys_storage
     - :doc:`Interior Point - Linear System Memory Usage <Interior Point/KNITRO_IP_-_Linear_System_Memory_Usage>`
   * - bar_maxcorrectors
     - :doc:`Interior Point - Barrier Corrector Steps Limit <Interior Point/KNITRO_IP_-_Barrier_Corrector_Steps_Limit>`
   * - bar_maxcrossit
     - :doc:`Interior Point - Crossover Iterations Limit <Interior Point/KNITRO_IP_-_CrossoverIterLimit>`
   * - bar_maxmu
     - :doc:`Interior Point - Barrier Maximum Mu <Interior Point/KNITRO_IP_-_Barrier_Maximum_Mu>`
   * - bar_maxrefactor
     - :doc:`Interior Point - Refactorization Limit <Interior Point/KNITRO_IP_-_RefactorizationLim>`
   * - bar_mpec_heuristic
     - :doc:`Interior Point - Barrier MPEC Heuristic <Interior Point/KNITRO_IP_-_Barrier_MPEC_Heuristic>`
   * - bar_murule
     - :doc:`Interior Point - Barrier Parameter Strategy <Interior Point/KNITRO_IP_-_Bar_Par_Strategy>`
   * - bar_penaltycons
     - :doc:`Interior Point - Barrier Penalty Constraint Strategy <Interior Point/KNITRO_IP_-_Barrier_Penalty_Constraint_St>`
   * - bar_penaltyrule
     - :doc:`Interior Point - Barrier Penalty Parameter Strategy <Interior Point/KNITRO_IP_-_Barrier_Penalty_Parameter_St>`
   * - bar_refinement
     - :doc:`Interior Point - Barrier Refinement <Interior Point/KNITRO_IP_-_Barrier_Refinement>`
   * - bar_relaxcons
     - :doc:`Interior Point - Barrier Relax Constraints <Interior Point/KNITRO_IP_-_Barrier_Relax_Constraints>`
   * - bar_slackboundpush
     - :doc:`Interior Point - Barrier Slack Bound Push <Interior Point/KNITRO_IP_-_Barrier_Slack_Bound_Push>`
   * - bar_switchobj
     - :doc:`Interior Point - Barrier Switch Objective <Interior Point/KNITRO_IP_-_Barrier_Switch_Objective>`
   * - bar_switchrule
     - :doc:`Interior Point - Barrier Switch Rule <Interior Point/KNITRO_IP_-_Barrier_Switch_Rule>`
   * - bar_watchdog
     - :doc:`Interior Point - Barrier Watchdog <Interior Point/KNITRO_IP_-_Barrier_Watchdog>`
   * - blas_numthreads
     - :doc:`Parallel - Number of BLAS Threads <Parallel/KNITRO_Par_-_Number_of_BLAS_threads>`
   * - blasoption
     - :doc:`General - BLAS Option <General/KNITRO_General_-_BLAS_Option>`
   * - cg_maxit
     - :doc:`Interior Point - Conjugate Gradient Iteration Limit <Interior Point/KNITRO_IP_-_ConjugateGradIter>`
   * - cg_pmem
     - :doc:`Interior Point - Conjugate Gradient Memory Limit <Interior Point/KNITRO_IP_-_Conjugate_Gradient_Memory_Limit>`
   * - cg_precond
     - :doc:`Interior Point - Conjugate Gradient Preconditioner <Interior Point/KNITRO_IP_-_Conjugate_Gradient_Preconditio>`
   * - cg_stoptol
     - :doc:`Interior Point - Conjugate Gradient Stopping Tolerance <Interior Point/KNITRO_IP_-_Conjugate_Gradient_Stopping_To>`
   * - convex
     - :doc:`General - Mark as Convex <General/KNITRO_General_-_Mark_as_Convex>`
   * - datacheck
     - :doc:`Debugging - Data Check <Debugging/KNITRO_Deb_-_Data_Check>`
   * - debug
     - :doc:`Debugging - Debugging Output <Debugging/KNITRO_Deb_-_DebuggingOutput>`
   * - delta
     - :doc:`Advanced - Initial Trust Scaling Factor <Advanced/KNITRO_Advanced_-_Initial_trust>`
   * - feastol
     - :doc:`Tolerances - Relative Feasibility Tolerance <Tolerances/KNITRO_Tol_-_RelFeasTol>`
   * - feastol_abs
     - :doc:`Tolerances - Absolute Feasibility Tolerance <Tolerances/KNITRO_Tol_-_AbsFeasTol>`
   * - findiff_estnoise
     - :doc:`Advanced - Estimate Noise in the Model <Advanced/KNITRO_Advanced_-_Estimate_Noise_in_the_Model>`
   * - findiff_numthreads
     - :doc:`Parallel - Number of Gradient Computation Threads <Parallel/KNITRO_Par_-_Number_of_Gradient_Computation_Threads>`
   * - fstopval
     - :doc:`Termination - Objective Goal <Termination/KNITRO_Term_-_Objective_Goal>`
   * - ftol
     - :doc:`Termination - Relative Improvement Tolerance <Termination/KNITRO_Term_-_Relative_Improvement_Tolerance>`
   * - ftol_iters
     - :doc:`Termination - Relative Improvement Iterations <Termination/KNITRO_Term_-_Relative_Improvement_Iterations>`
   * - gradopt
     - :doc:`Advanced - Gradient Computation Method <Advanced/KNITRO_Advanced_-_Gradient_Computation_Method>`
   * - hessopt
     - :doc:`Hessian - Hessian Computation Method <Hessian/KNITRO_Hessian_-_Hes_Comp_Meth>`
   * - honorbnds
     - :doc:`General - Honor Bounds <General/KNITRO_General_-_Honor_Bounds>`
   * - infeastol
     - :doc:`Tolerances - Infeasibility Tolerance <Tolerances/KNITRO_Tol_-_Infeasibility_Tolerance>`
   * - infeastol_iters
     - :doc:`Termination - Infeasibility Tolerance Iteration Limit <Termination/KNITRO_Term_-_Infeas_Tol_Iteration_Limit>`
   * - initpenalty
     - :doc:`Advanced - Initial Penalty Value <Advanced/KNITRO_Advanced_-_Initial_Penalty_Value>`
   * - linesearch
     - :doc:`Advanced - Linesearch Strategy <Advanced/KNITRO_Advanced_-_Linesearch_Strategy>`
   * - linesearch_maxtrials
     - :doc:`Advanced - Linesearch Trials Limit <Advanced/KNITRO_Advanced_-_Linesearch_Trials_Limit>`
   * - linsolver
     - :doc:`General - Linear Solver <General/KNITRO_General_-_Linear_Solver>`
   * - linsolver_maxitref
     - :doc:`General - Linear System Max Iterative Refinements <General/KNITRO_General_-_Linear_System_Max_Iterative_Re>`
   * - linsolver_nodeamalg
     - :doc:`General - Linear Solver Node Amalgamation <General/KNITRO_General_-_Linear_Solver_Node_Amalgamation>`
   * - linsolver_numthreads
     - :doc:`Parallel - Number of Linear System Threads <Parallel/KNITRO_Par_-_Number_of_Lin_Sys_Threads>`
   * - linsolver_ooc
     - :doc:`General - Linear Solver Out of Core <General/KNITRO_General_-_Linear_Solver_Out_of_Core>`
   * - linsolver_ordering
     - :doc:`General - Linear Solver Ordering <General/KNITRO_General_-_Linear_Solver_Ordering>`
   * - linsolver_pivottol
     - :doc:`Advanced - Initial Pivot Treshold <Advanced/KNITRO_Advanced_-_Initial_pivot>`
   * - linsolver_scaling
     - :doc:`General - Linear Solver Scaling <General/KNITRO_General_-_Linear_Solver_Scaling>`
   * - lmsize
     - :doc:`Hessian - Limited Memory Size <Hessian/KNITRO_Hessian_-_Limited_Memory_Size>`
   * - ma_outsub
     - :doc:`Reporting - Multi Algorithm Output <Reporting/KNITRO_Reporting_-_Multi_Algorithm_Output>`
   * - ma_terminate
     - :doc:`Termination - Multi Algorithm Termination <Termination/KNITRO_Term_-_Multi_Algorithm_Termination>`
   * - maxfevals
     - :doc:`Termination - Function Evaluations Limit <Termination/KNITRO_Term_-_Function_Evaluations_Limit>`
   * - maxit
     - :doc:`Stop Criteria - Iteration Limit <../../Aimms/Options/Solvers General/Stop Criteria/Stop_Criteria_-_Iteration_Limi>`  in 'Solvers general'
   * - maxtime_cpu
     - :doc:`Stop Criteria - Time Limit <../../Aimms/Options/Solvers General/Stop Criteria/Stop_Criteria_-_Time_Limit>`  in 'Solvers general'
   * - mip_branchrule
     - :doc:`MIP - MIP Branching Rule <MIP/KNITRO_MIP_-_MIP_Branching_Rule>`
   * - mip_clique
     - :doc:`MIP Cuts - Clique Cuts <MIP Cuts/KNITRO_MIP_Cuts_-_Clique_cuts>`
   * - mip_cut_flowcover
     - :doc:`MIP Cuts - Flow Cover Cuts <MIP Cuts/KNITRO_MIP_Cuts_-_Flowcover_Cuts>`
   * - mip_cut_probing
     - :doc:`MIP Cuts - Probing Cuts <MIP Cuts/KNITRO_MIP_Cuts_-_Probing_Cuts>`
   * - mip_cutoff
     - :doc:`MIP - MIP Objective Cutoff Value <MIP/KNITRO_MIP_-_MIP_Objective_Cutoff_Value>`
   * - mip_debug
     - :doc:`Debugging - Debugging MIP output <Debugging/KNITRO_Deb_-_Debugging_MIP_output>`
   * - mip_gomory
     - :doc:`MIP Cuts - Gomory Cuts <MIP Cuts/KNITRO_MIP_Cuts_-_Gomory_Cuts>`
   * - mip_gub_branch
     - :doc:`MIP - MIP GUB Branch <MIP/KNITRO_MIP_-_MIP_GUB_Branch>`
   * - mip_heuristic
     - :doc:`MIP - MIP Heuristic <MIP/KNITRO_MIP_-_MIP_Heuristic>`
   * - mip_heuristic_diving
     - :doc:`MIP - MIP Heuristic Diving <MIP/KNITRO_MIP_-_MIP_Heuristic_Diving>`
   * - mip_heuristic_feaspump
     - :doc:`MIP - MIP Heuristic Feasibility Pump <MIP/KNITRO_MIP_-_MIP_Heuristic_Feasibility_Pump>`
   * - mip_heuristic_lns
     - :doc:`MIP - MIP Heuristic Large Neighborhood Search <MIP/KNITRO_MIP_-_MIP_Heuristic_Large_Neighborhood_Search>`
   * - mip_heuristic_localsearch
     - :doc:`MIP - MIP Heuristic Local Search <MIP/KNITRO_MIP_-_MIP_Heuristic_Local_Search>`
   * - mip_heuristic_maxit
     - :doc:`MIP - MIP Heuristic Iteration Limit <MIP/KNITRO_MIP_-_MIP_Heuristic_Iteration_Limit>`
   * - mip_heuristic_misqp
     - :doc:`MIP - MIP MISQP Heuristic <MIP/KNITRO_MIP_-_MIP_MISQP_Heuristic>`
   * - mip_heuristic_mpec
     - :doc:`MIP - MIP Heuristic MPEC <MIP/KNITRO_MIP_-_MIP_Heuristic_MPEC>`
   * - mip_heuristic_strategy
     - :doc:`MIP - MIP Heuristic Strategy <MIP/KNITRO_MIP_-_MIP_Heuristic_Strategy>`
   * - mip_heuristic_terminate
     - :doc:`MIP - MIP Heuristic Terminate <MIP/KNITRO_MIP_-_MIP_Heuristic_Terminate>`
   * - mip_implications
     - :doc:`MIP - MIP Implications <MIP/KNITRO_MIP_-_MIP_Implications>`
   * - mip_integer_tol
     - :doc:`MIP - Integrality <MIP/KNITRO_MIP_-_Integrality>`
   * - mip_intvar_strategy
     - :doc:`MIP - MIP Integer Variables Strategy <MIP/KNITRO_MIP_-_MIP_Integer_Variables_Strategy>`
   * - mip_knapsack
     - :doc:`MIP Cuts - Knapsack Cuts <MIP Cuts/KNITRO_MIP_Cuts_-_Knapsack_cuts>`
   * - mip_liftproject
     - :doc:`MIP Cuts - Lift and Project Cuts <MIP Cuts/KNITRO_MIP_Cuts_-_Lift_and_Project_Cuts>`
   * - mip_lpalg
     - :doc:`MIP - MIP Algorithm <MIP/KNITRO_MIP_-_MIP_Algorithm>`
   * - mip_maxnodes
     - :doc:`MIP - Maximal Number of Nodes <MIP/KNITRO_MIP_-_Maximal_Number_of_Nodes>`
   * - mip_maxsolves
     - :doc:`MIP - Maximal Number of Subproblem Solves <MIP/KNITRO_MIP_-_Maximal_Nr_Subproblem_Slvs>`
   * - mip_method
     - :doc:`MIP - MIP Method <MIP/KNITRO_MIP_-_MIP_Method>`
   * - mip_mir
     - :doc:`MIP Cuts - MIR Cuts <MIP Cuts/KNITRO_MIP_Cuts_-_MIR_cuts>`
   * - mip_multistart
     - :doc:`MIP - MIP Multistart <MIP/KNITRO_MIP_-_MIP_Multistart>`
   * - mip_nodealg
     - :doc:`MIP - Node Algorithm <MIP/KNITRO_MIP_-_Node_Algorithm>`
   * - mip_numthreads
     - :doc:`Parallel - Number of MIP Threads <Parallel/KNITRO_Par_-_Number_of_MIP_Threads>`
   * - mip_outinterval
     - :doc:`Reporting - MIP Output Level <Reporting/KNITRO_Reporting_-_MIP_Output_Level>`
   * - mip_pseudoinit
     - :doc:`MIP - MIP Pseudo Cost Initialization <MIP/KNITRO_MIP_-_MIP_Pseudo_Cost_Initialization>`
   * - mip_relaxable
     - :doc:`MIP - MIP Integer Variables Relaxable <MIP/KNITRO_MIP_-_MIP_Integer_Variables_Relaxabl>`
   * - mip_restart
     - :doc:`MIP - MIP Restart <MIP/KNITRO_MIP_-_MIP_Restart>`
   * - mip_rootalg
     - :doc:`MIP - MIP Start Algorithm <MIP/KNITRO_MIP_-_MIP_Start_Algorithm>`
   * - mip_rounding
     - :doc:`MIP - MIP Rounding <MIP/KNITRO_MIP_-_MIP_Rounding>`
   * - mip_selectdir
     - :doc:`MIP - Node Selection_Direction <MIP/KNITRO_MIP_-_Node_Selection_Direction>`
   * - mip_selectrule
     - :doc:`MIP - Node Selection <MIP/KNITRO_MIP_-_Node_Selection>`
   * - mip_strong_candlim
     - :doc:`MIP - Strong Branching Candidates Limit <MIP/KNITRO_MIP_-_Strong_Branch_Candidates_Limit>`
   * - mip_strong_level
     - :doc:`MIP - Strong Branching Level <MIP/KNITRO_MIP_-_Strong_Branching_Level>`
   * - mip_strong_maxit
     - :doc:`MIP - Strong Branching Iteration Limit <MIP/KNITRO_MIP_-_Strong_Branch_Iter_Limit>`
   * - mip_terminate
     - :doc:`MIP - MIP Terminate <MIP/KNITRO_MIP_-_MIP_Terminate>`
   * - mip_zerohalf
     - :doc:`MIP Cuts - Zero Half Cuts <MIP Cuts/KNITRO_MIP_Cuts_-_Zero_Half_cuts>`
   * - ms_deterministic
     - :doc:`Multistart - Multistart Deterministic <Multistart/KNITRO_MS_-_Multistart_Deterministic>`
   * - ms_enable
     - :doc:`Multistart - Multistart <Multistart/KNITRO_MS_-_Multistart>`
   * - ms_intpt_cluster
     - :doc:`Multistart - Multistart Initial Points Cluster <Multistart/KNITRO_MS_-_Multistart_Initial_Points_Clus>`
   * - ms_maxbndrange
     - :doc:`Multistart - Multistart Range Unbounded Variable <Multistart/KNITRO_MS_-_Multistart_Range_Unbounded_Var>`
   * - ms_maxsolves
     - :doc:`Multistart - Number of Multistart Points <Multistart/KNITRO_MS_-_Nr_multi_points>`
   * - ms_num_to_save
     - :doc:`Multistart - Number of Best Solutions <Multistart/KNITRO_MS_-_Number_of_Best_Solutions>`
   * - ms_numthreads
     - :doc:`Parallel - Number of Multistart Threads <Parallel/KNITRO_Par_-_Number_of_Multistart_Threads>`
   * - ms_savetol
     - :doc:`Multistart - Solution Distance <Multistart/KNITRO_MS_-_Solution_Distance>`
   * - ms_seed
     - :doc:`Multistart - Multistart Seed <Multistart/KNITRO_MS_-_Multistart_Seed>`
   * - ms_startptrange
     - :doc:`Multistart - Multistart Range <Multistart/KNITRO_MS_-_Multistart_Range>`
   * - ms_terminate
     - :doc:`Multistart - Multistart Termination Condition <Multistart/KNITRO_MS_-_MS_Termination_Conditi>`
   * - ncvx_qcqp_init
     - :doc:`Advanced - QP and QCQP Initialization Strategy <Advanced/KNITRO_Advanced_-_QP_and_QCQP_Initialization_Str>`
   * - numthreads
     - :doc:`Parallel - Number of Threads <Parallel/KNITRO_Par_-_Number_of_Threads>`
   * - objrange
     - :doc:`General - Unboundedness Range <General/KNITRO_General_-_Unbound_range>`
   * - opttol
     - :doc:`Termination - Relative Optimality Tolerance <Termination/KNITRO_Term_-_RelOptTol>`
   * - opttol_abs
     - :doc:`Termination - Absolute Optimality Tolerance <Termination/KNITRO_Term_-_AbsOptTol>`
   * - outlev
     - :doc:`Reporting - Status File Display <Reporting/KNITRO_Reporting_-_StatusFileDi>`
   * - numthreads
     - :doc:`Parallel - Number of Threads <Parallel/KNITRO_Par_-_Number_of_Threads>`
   * - presolve
     - :doc:`Presolve - Presolve <Presolve/KNITRO_Presolve_-_Presolve>`
   * - presolve_initpt
     - :doc:`Presolve - Presolve Initial Point <Presolve/KNITRO_Presolve_-_Presolve_Initial_Point_Shift>`
   * - presolve_level
     - :doc:`Presolve - Presolve Level <Presolve/KNITRO_Presolve_-_Presolve_Level>`
   * - presolve_passes
     - :doc:`Presolve - Presolve Passes <Presolve/KNITRO_Presolve_-_Presolve_Passes>`
   * - presolve_tol
     - :doc:`Presolve - Presolve Tolerance <Presolve/KNITRO_Presolve_-_Presolve_Tolerance>`
   * - presolveop_redundant
     - :doc:`Presolve - Presolve Redundant Constraints <Presolve/KNITRO_Presolve_-_Presolve_Redundant_Constraints>`
   * - presolveop_substitution
     - :doc:`Presolve - Presolve Substitution <Presolve/KNITRO_Presolve_-_Presolve_Substitution>`
   * - presolveop_substitution_tol
     - :doc:`Presolve - Presolve Substitution Tolerance <Presolve/KNITRO_Presolve_-_Presolve_Substitution_Tolerance>`
   * - presolveop_tighten
     - :doc:`Presolve - Tighten Variable Bounds <Presolve/KNITRO_Presolve_-_Tighten_Variable_Bounds>`
   * - restarts
     - :doc:`General - Restarts <General/KNITRO_General_-_Restarts>`
   * - restarts_maxit
     - :doc:`General - Restarts Iteration Limit <General/KNITRO_General_-_Restarts_Iteration_Limit>`
   * - scale
     - :doc:`General - Scaling <General/KNITRO_General_-_Scaling>`
   * - scale_vars
     - :doc:`General - Scale Variables <General/KNITRO_General_-_Scale_Variables>`
   * - soc
     - :doc:`Hessian - Second Order Correction <Hessian/KNITRO_Hessian_-_SecondOrderCor>`
   * - strat_warm_start
     - :doc:`General - Warm Start Strategy <General/KNITRO_General_-_Warm_Start_Strategy>`
   * - tuner
     - :doc:`Tuner - Tuner <Tuner/KNITRO_Tuner_-_Tuner>`
   * - tuner_maxtime_cpu
     - :doc:`Tuner - Tuner Time Limit <Tuner/KNITRO_Tuner_-_Tuner_Time_Limit>`
   * - tuner_outsub
     - :doc:`Tuner - Tuner Output <Tuner/KNITRO_Tuner_-_Tuner_Output>`
   * - tuner_terminate
     - :doc:`Tuner - Tuner Terminate <Tuner/KNITRO_Tuner_-_Tuner_Terminate>`
   * - xtol
     - :doc:`Advanced - Solution Progress Tolerance <Advanced/KNITRO_Advanced_-_SolutionProgressTol>`
   * - xtol_iters
     - :doc:`Advanced - Solution Progress Iterations <Advanced/KNITRO_Advanced_-_Solution_Progress_Iterations>`
