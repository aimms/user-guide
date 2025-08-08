

.. _AIMMS_to_KNITRO_Mapping:
.. _KNITRO_AIMMS_to_KNITRO_Mapping:


AIMMS to Knitro 14.0 Mapping
============================

**Description** 

The table shows in the left column the AIMMS Knitro options; the right column displays for the AIMMS option the Knitro option that is associated with it.



**Option name in AIMMS** 		**Name in Knitro** 	

:ref:`KNITRO_Advanced_-_Estimate_Noise_in_the_Model` 		findiff_estnoise	

:ref:`KNITRO_Advanced_-_Gradient_Computation_Method` 		gradopt	

:ref:`KNITRO_Advanced_-_Initial_Penalty_Value` 		initpenalty

:ref:`KNITRO_Advanced_-_Initial_pivot` 		linsolver_pivottol	

:ref:`KNITRO_Advanced_-_Initial_trust` 		delta	

:ref:`KNITRO_Advanced_-_Linesearch_Strategy` 		linesearch

:ref:`KNITRO_Advanced_-_Linesearch_Trials_Limit` 		linesearch_maxtrials

:ref:`KNITRO_Advanced_-_LP_Algorithm`  		act_lpalg

:ref:`KNITRO_Advanced_-_Objective_Reduction`  		act_lppenalty

:ref:`KNITRO_Advanced_-_LP_Presolve`  		act_lppresolve

:ref:`KNITRO_Advanced_-_Objective_Reduction`  	

:ref:`KNITRO_Advanced_-_QP_and_QCQP_Initialization_Str`   		ncvx_qcqp_init

:ref:`KNITRO_Advanced_-_Solution_Progress_Iterations`   		xtol_iters

:ref:`KNITRO_Advanced_-_SolutionProgressTol`   		xtol

:ref:`KNITRO_Deb_-_Data_Check` 		datacheck

:ref:`KNITRO_Deb_-_Debugging_MIP_output` 		mip_debug

:ref:`KNITRO_Deb_-_DebuggingOutput` 		debug

:ref:`KNITRO_General_-_Act_QPpenalty` 		act_qppenalty

:ref:`KNITRO_General_-_Algorithm` 		algorithm	

:ref:`KNITRO_General_-_BLAS_Option`  		blasoption	

:ref:`KNITRO_General_-_Honor_Bounds`  		honorbnds	

:ref:`KNITRO_General_-_Linear_Solver`  		linsolver	

:ref:`KNITRO_General_-_Linear_Solver_Node_Amalgamation`  		linsolver_nodeamalg	

:ref:`KNITRO_General_-_Linear_Solver_Ordering`  		linsolver_ordering	

:ref:`KNITRO_General_-_Linear_Solver_Out_of_Core`  		linsolver_ooc	

:ref:`KNITRO_General_-_Linear_Solver_Scaling`  		linsolver_scaling

:ref:`KNITRO_General_-_Linear_System_Max_Iterative_Re` 		linsolver_maxitref	

:ref:`KNITRO_General_-_LP_Solver` 		act_lpsolver

:ref:`KNITRO_General_-_Mark_as_Convex` 		convex

:ref:`KNITRO_General_-_QP_Algorithm` 		act_qpalg		

:ref:`KNITRO_General_-_Restarts`  		restarts

:ref:`KNITRO_General_-_Restarts_Iteration_Limit`  		restarts_maxit

:ref:`KNITRO_General_-_Scale_Variables` 		scale_vars	

:ref:`KNITRO_General_-_Scaling` 		scale	

:ref:`KNITRO_General_-_Unbound_range`  		objrange	

:ref:`KNITRO_General_-_Use_initial_so`  	

:ref:`KNITRO_General_-_Warm_Start_Strategy`  		strat_warm_start

:ref:`KNITRO_Hessian_-_Hes_Comp_Meth` 		hessopt	

:ref:`KNITRO_Hessian_-_Limited_Memory_Size`  		lmsize	

:ref:`KNITRO_Hessian_-_SecondOrderCor`  		soc		

:ref:`KNITRO_IP_-_Barrier_Corrector_Steps_Limit`  		bar_maxcorrectors	

:ref:`KNITRO_IP_-_Barrier_Enable_Conic`  		bar_conic_enable

:ref:`KNITRO_IP_-_Barrier_Globalize`  		bar_globalize

:ref:`KNITRO_IP_-_Barrier_Maximum_Mu`  		bar_maxmu

:ref:`KNITRO_IP_-_Barrier_MPEC_Heuristic`  		bar_mpec_heuristic

:ref:`KNITRO_IP_-_Bar_Par_Strategy`  		bar_murule	

:ref:`KNITRO_IP_-_Barrier_Penalty_Constraint_St`  		bar_penaltycons	

:ref:`KNITRO_IP_-_Barrier_Penalty_Parameter_St`  		bar_penaltyrule			

:ref:`KNITRO_IP_-_Barrier_Refinement`  		bar_refinement

:ref:`KNITRO_IP_-_Barrier_Relax_Constraints`  		bar_relaxcons

:ref:`KNITRO_IP_-_Barrier_Slack_Bound_Push`  		bar_slackboundpush

:ref:`KNITRO_IP_-_Barrier_Switch_Objective` 		bar_switchobj

:ref:`KNITRO_IP_-_Barrier_Switch_Rule`  		bar_switchrule

:ref:`KNITRO_IP_-_Barrier_Watchdog`  		bar_watchdog

:ref:`KNITRO_IP_-_ConjugateGradIter`  		cg_maxit	

:ref:`KNITRO_IP_-_Conjugate_Gradient_Memory_Limit` 		cg_pmem

:ref:`KNITRO_IP_-_Conjugate_Gradient_Preconditio` 		cg_precond

:ref:`KNITRO_IP_-_Conjugate_Gradient_Stopping_To` 		cg_stoptol

:ref:`KNITRO_IP_-_CrossoverIterLimit`  		bar_maxcrossit	

:ref:`KNITRO_IP_-_Direct_Step_Interval`  		bar_directinterval	

:ref:`KNITRO_IP_-_Feasible_mode`  		bar_feasible	

:ref:`KNITRO_IP_-_Feas_mode_act_tol`  		bar_feasmodetol	

:ref:`KNITRO_IP_-_InitBarParValue` 		bar_initmu	

:ref:`KNITRO_IP_-_Initial_Barrier_Penalty_Value`  		bar_initpi_mpec

:ref:`KNITRO_IP_-_Initial_Point_Strat`  		bar_initpt

:ref:`KNITRO_IP_-_Linear_System_Form_Used` 		bar_linsys	

:ref:`KNITRO_IP_-_Linear_System_Memory_Usage` 		bar_linsys_storage	

:ref:`KNITRO_IP_-_RefactorizationLim`  		bar_maxrefactor		

:ref:`KNITRO_MIP_-_Integrality`   		mip_integer_tol

:ref:`KNITRO_MIP_-_Maximal_Number_of_Nodes`   		mip_maxnodes

:ref:`KNITRO_MIP_-_Maximal_Nr_Subproblem_Slvs`   		mip_maxsolves

:ref:`KNITRO_MIP_-_MIP_Algorithm`   		mip_lpalg

:ref:`KNITRO_MIP_-_MIP_Branching_Rule`   		mip_branchrule

:ref:`KNITRO_MIP_-_MIP_GUB_Branch`   		mip_gub_branch

:ref:`KNITRO_MIP_-_MIP_Heuristic`   		mip_heuristic

:ref:`KNITRO_MIP_-_MIP_Heuristic_Diving`   		mip_heuristic_diving

:ref:`KNITRO_MIP_-_MIP_Heuristic_Feasibility_Pump`   		mip_heuristic_feaspump

:ref:`KNITRO_MIP_-_MIP_Heuristic_Iteration_Limit`   		mip_heuristic_maxit

:ref:`KNITRO_MIP_-_MIP_Heuristic_Large_Neighborhood_Search`   		mip_heuristic_lns

:ref:`KNITRO_MIP_-_MIP_Heuristic_Local_Search`   		mip_heuristic_local_search

:ref:`KNITRO_MIP_-_MIP_Heuristic_MPEC`   		mip_heuristic_mpec

:ref:`KNITRO_MIP_-_MIP_Heuristic_Strategy`   		mip_heuristic_strategy

:ref:`KNITRO_MIP_-_MIP_Heuristic_Terminate`   		mip_heuristic_terminate

:ref:`KNITRO_MIP_-_MIP_Implications`  		mip_implications

:ref:`KNITRO_MIP_-_MIP_Integer_Variables_Relaxabl`  		mip_relaxable

:ref:`KNITRO_MIP_-_MIP_Integer_Variables_Strategy`  		mip_intvar_strategy

:ref:`KNITRO_MIP_-_MIP_Method`   		mip_method	

:ref:`KNITRO_MIP_-_MIP_MISQP_Heuristic`   		mip_heuristic_misqp	

:ref:`KNITRO_MIP_-_MIP_Multistart`   		mip_multistart	

:ref:`KNITRO_MIP_-_MIP_Objective_Cutoff_Value`   		mip_cutoff	

:ref:`KNITRO_MIP_-_MIP_Pseudo_Cost_Initialization`   		mip_pseudoinit

:ref:`KNITRO_MIP_-_MIP_Restart`   		mip_restart

:ref:`KNITRO_MIP_-_MIP_Rounding`   		mip_rounding

:ref:`KNITRO_MIP_-_MIP_Start_Algorithm`   		mip_rootalg

:ref:`KNITRO_MIP_-_MIP_Terminate`   		mip_terminate

:ref:`KNITRO_MIP_-_Node_Algorithm`   		mip_nodealg

:ref:`KNITRO_MIP_-_Node_Selection`   		mip_selectrule

:ref:`KNITRO_MIP_-_Node_Selection_Direction`   		mip_selectdir

:ref:`KNITRO_MIP_-_Strong_Branch_Candidates_Limit`    		mip_strong_candlim

:ref:`KNITRO_MIP_-_Strong_Branch_Iter_Limit`   		mip_strong_maxit

:ref:`KNITRO_MIP_-_Strong_Branching_Level`   		mip_strong_level

:ref:`KNITRO_MIP_Cuts_-_Clique_cuts`   		mip_clique

:ref:`KNITRO_MIP_Cuts_-_Flowcover_Cuts`   		mip_cut_flowcover

:ref:`KNITRO_MIP_Cuts_-_Gomory_Cuts`   		mip_gomory

:ref:`KNITRO_MIP_Cuts_-_Knapsack_cuts`   		mip_knapsack

:ref:`KNITRO_MIP_Cuts_-_Lift_and_Project_Cuts`   		mip_liftproject

:ref:`KNITRO_MIP_Cuts_-_MIR_cuts`   		mip_mir

:ref:`KNITRO_MIP_Cuts_-_Probing_Cuts`   		mip_cut_probing

:ref:`KNITRO_MIP_Cuts_-_Zero_Half_cuts`   		mip_zerohalf

:ref:`KNITRO_MS_-_Multistart` 		ms_enable	

:ref:`KNITRO_MS_-_Multistart_Deterministic` 		ms_deterministic

:ref:`KNITRO_MS_-_Multistart_Initial_Points_Clus` 		ms_initpt_cluster

:ref:`KNITRO_MS_-_Multistart_Range` 		ms_startptrange	

:ref:`KNITRO_MS_-_Multistart_Range_Unbounded_Var` 		ms_maxbndrange	

:ref:`KNITRO_MS_-_Multistart_Seed` 		ms_seed	

:ref:`KNITRO_MS_-_MS_Single_Solve_Tim` 	

:ref:`KNITRO_MS_-_MS_Termination_Conditi` 		ms_terminate

:ref:`KNITRO_MS_-_Number_of_Best_Solutions`  		ms_num_to_save	

:ref:`KNITRO_MS_-_Nr_multi_points`  		ms_maxsolves	

:ref:`KNITRO_MS_-_Solution_Distance`  		ms_savetol	

:ref:`KNITRO_Par_-_Number_of_Gradient_Computation_Threads` 		findiff_numthreads

:ref:`KNITRO_Par_-_Number_of_BLAS_threads` 		blas_numthreads

:ref:`KNITRO_Par_-_Number_of_Lin_Sys_Threads` 		linsolver_numthreads

:ref:`KNITRO_Par_-_Number_of_MIP_Threads` 		mip_numthreads

:ref:`KNITRO_Par_-_Number_of_Multistart_Threads` 		ms_numthreads

:ref:`KNITRO_Par_-_Number_of_Threads` 		numthreads

:ref:`KNITRO_Presolve_-_Presolve`  		presolve	

:ref:`KNITRO_Presolve_-_Presolve_Identify_Lin_Var`  	

:ref:`KNITRO_Presolve_-_Presolve_Initial_Point_Shift` 		presolve_initpt	

:ref:`KNITRO_Presolve_-_Presolve_Level`  		presolve_level

:ref:`KNITRO_Presolve_-_Presolve_Passes`  		presolve_passes

:ref:`KNITRO_Presolve_-_Presolve_Redundant_Constraints`  		presolveop_redundant

:ref:`KNITRO_Presolve_-_Presolve_Substitution`  		presolveop_substitution

:ref:`KNITRO_Presolve_-_Presolve_Substitution_Tolerance`  		presolveop_substitution_tol

:ref:`KNITRO_Presolve_-_Presolve_Tolerance`  		presolve_tol	

:ref:`KNITRO_Presolve_-_Tighten_Variable_Bounds`  		presolveop_tighten

:ref:`KNITRO_Reporting_-_MIP_Output_Level`  		mip_outinterval	

:ref:`KNITRO_Reporting_-_Multi_Algorithm_Output`  		ma_outsub

:ref:`KNITRO_Reporting_-_StatusFileDi`  		outlev	

:ref:`KNITRO_Term_-_AbsOptTol`  		opttol_abs

:ref:`KNITRO_Term_-_Function_Evaluations_Limit`  		maxfevals

:ref:`KNITRO_Term_-_Infeas_Tol_Iteration_Limit`  		infeastol_iters	

:ref:`KNITRO_Term_-_Multi_Algorithm_Termination`  		ma_terminate

:ref:`KNITRO_Term_-_Objective_Goal`  		fstopval

:ref:`KNITRO_Term_-_Relative_Improvement_Iterations`  		ftol_iters	

:ref:`KNITRO_Term_-_Relative_Improvement_Tolerance`  		ftol	

:ref:`KNITRO_Term_-_RelOptTol`  		opttol	

:ref:`KNITRO_Tol_-_AbsFeasTol` 		feastol_abs		

:ref:`KNITRO_Tol_-_Infeasibility_Tolerance`  		infeastol	

:ref:`KNITRO_Tol_-_LP_Feasibility_Tolerance`  		act_lpfeastol

:ref:`KNITRO_Tol_-_Marginals_Tol`  	

:ref:`KNITRO_Tol_-_RelFeasTol` 		feastol	

:ref:`KNITRO_Tuner_-_Tuner`  		tuner	

:ref:`KNITRO_Tuner_-_Tuner_Output`  		tuner_outsub	

:ref:`KNITRO_Tuner_-_Tuner_Terminate`  		tuner_terminate	

:ref:`KNITRO_Tuner_-_Tuner_Time_Limit`  		tuner_maxtime_cpu	

	

