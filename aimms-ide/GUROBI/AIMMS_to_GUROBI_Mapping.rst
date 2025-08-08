

.. _AIMMS_to_GUROBI_Mapping:
.. _GUROBI_AIMMS_to_GUROBI_Mapping:


AIMMS to GUROBI Mapping
============================

**Description** 

The table shows in the left column the AIMMS Gurobi options while the right column displays the associated Gurobi parameter.




.. list-table::

   * - **Option name in AIMMS** 
     - **Name in GUROBI** 
   * - :ref:`GUROBI_Barrier_-_Barrier_Convergence_Tolerance` 
     - BARCONVTOL
   * - :ref:`GUROBI_Barrier_-_Barrier_Correction_Steps` 
     - BARCORRECTORS
   * - :ref:`GUROBI_Barrier_-_Barrier_Crossover` 
     - CROSSOVER
   * - :ref:`GUROBI_Barrier_-_Barrier_Crossover_Basis` 
     - CROSSOVERBASIS
   * - :ref:`GUROBI_Barrier_-_Barrier_Homogeneous_Aalgorithm` 
     - BARHOMOGENEOUS
   * - :ref:`GUROBI_Barrier_-_Barrier_Iteration_Limit` 
     - BARITERLIMIT
   * - :ref:`GUROBI_Barrier_-_Barrier_Ordering` 
     - BARORDER
   * - :ref:`GUROBI_Barrier_-_Barrier_Progress_Solution` 
     - 
   * - :ref:`GUROBI_Barrier_-_Barrier_QCP_Convergence_Tol` 
     - BARQCPCONVTOL
   * - :ref:`GUROBI_General_-_Calculate_Kappa` 
     - 
   * - :ref:`GUROBI_General_-_Concurrent_Method` 
     - CONCURRENTMETHOD
   * - :ref:`GUROBI_General_-_Farkas_Infeasibility_Proof`  
     - 
   * - :ref:`GUROBI_General_-_Feasibility`  
     - FEASIBILITYTOL
   * - :ref:`GUROBI_General_-_IIS_Method` 
     - FEASRELAXBIGM
   * - :ref:`GUROBI_General_-_IIS_Method`  
     - IISMETHOD
   * - :ref:`GUROBI_General_-_Memory_Limit` 
     - MEMLIMIT
   * - :ref:`GUROBI_General_-_Method`  
     - METHOD
   * - :ref:`GUROBI_General_-_MPS`  
     - 
   * - :ref:`GUROBI_General_-_MPS_Dual` 
     - 
   * - :ref:`GUROBI_General_-_Multi_objective_method`  
     - MULTIOBJMETHOD
   * - :ref:`GUROBI_General_-_Numeric_Focus`  
     - NUMERICFOCUS
   * - :ref:`GUROBI_General_-_Optimality`  
     - OPTIMALITYTOL
   * - :ref:`GUROBI_General_-_Random_Seed`  
     - SEED
   * - :ref:`GUROBI_General_-_Read_Parameter_File`  
     - 
   * - :ref:`GUROBI_General_-_Restart`  
     - 
   * - :ref:`GUROBI_General_-_Restart_File_Nr` 
     - 
   * - :ref:`GUROBI_General_-_Scale`  
     - SCALEFLAG
   * - :ref:`GUROBI_General_-_Sensitivity_Method`  
     - 
   * - :ref:`GUROBI_General_-_Soft_Memory_Limit` 
     - SOFTMEMLIMIT
   * - :ref:`GUROBI_General_-_Solution_File`  
     - 
   * - :ref:`GUROBI_General_-_Solution_Target`  
     - SOLUTIONTARGET
   * - :ref:`GUROBI_General_-_Unbounded_ray`  
     - 
   * - :ref:`GUROBI_General_-_Updates_Batch_Size`  
     - 
   * - :ref:`GUROBI_General_-_Warm_Start` 
     - LPWARMSTART
   * - :ref:`GUROBI_General_-_Work_Limit` 
     - WORKLIMIT
   * - :ref:`GUROBI_General_-_Write_Parameter_File` 
     - 
   * - :ref:`GUROBI_Logging_-_Display_Solution_Quality`  
     - 
   * - :ref:`GUROBI_Logging_-_Log_to_Console`  
     - LOGTOCONSOLE
   * - :ref:`GUROBI_Logging_-_Output_File`  
     - OUTPUTFLAG
   * - :ref:`GUROBI_Logging_-_Output_File_Display_Interval`  
     - DISPLAYINTERVAL
   * - :ref:`GUROBI_Logging_-_Tune_Output_Level`  
     - TUNEOUTPUT
   * - :ref:`GUROBI_MIP_-_Branch_direction`  
     - BRANCHDIR
   * - :ref:`GUROBI_MIP_-_Disconnected_Component_Strateg`  
     - DISCONNECTED
   * - :ref:`GUROBI_MIP_-_Hints_File`  
     - 
   * - :ref:`GUROBI_MIP_-_Improve_Start_Gap` 
     - IMPROVESTARTGAP
   * - :ref:`GUROBI_MIP_-_Improve_Start_Nodes` 
     - IMPROVESTARTNODES
   * - :ref:`GUROBI_MIP_-_Improve_Start_Time` 
     - IMPROVESTARTTIME
   * - :ref:`GUROBI_MIP_-_Integrality`  
     - INTFEASTOL
   * - :ref:`GUROBI_MIP_-_Integrality_Focus`  
     - INTEGRALITYFOCUS
   * - :ref:`GUROBI_MIP_-_Lazy_Constraint_Mode`  
     - 
   * - :ref:`GUROBI_MIP_-_MIP_Best_Bound_Stop`  
     - BESTBDSTOP
   * - :ref:`GUROBI_MIP_-_MIP_Best_Objective_Stop`  
     - BESTOBJSTOP
   * - :ref:`GUROBI_MIP_-_MIP_Focus`  
     - MIPFOCUS
   * - :ref:`GUROBI_MIP_-_MIP_Node_Method`  
     - NODEMETHOD
   * - :ref:`GUROBI_MIP_-_MIP_Start`  
     - 
   * - :ref:`GUROBI_MIP_-_MIP_Start_Node_Limit`  
     - STARTNODELIMIT
   * - :ref:`GUROBI_MIP_-_MIP_Symmetry`  
     - SYMMETRY
   * - :ref:`GUROBI_MIP_-_Node_File_Start`  
     - NODEFILESTART
   * - :ref:`GUROBI_MIP_-_Node_Limit`  
     - NODELIMIT
   * - :ref:`GUROBI_MIP_-_Select_Variables`  
     - VARBRANCH
   * - :ref:`GUROBI_MIP_Cuts_-_BQP_Cuts` 
     - BQPCUTS
   * - :ref:`GUROBI_MIP_Cuts_-_Clique_Cuts`  
     - CLIQUECUTS
   * - :ref:`GUROBI_MIP_Cuts_-_Cover_Cuts` 
     - COVERCUTS
   * - :ref:`GUROBI_MIP_Cuts_-_Dual_Implied_Cuts` 
     - DUALIMPLIEDCUTS
   * - :ref:`GUROBI_MIP_Cuts_-_Cut_Aggr_Passes_Limit` 
     - CUTAGGPASSES
   * - :ref:`GUROBI_MIP_Cuts_-_Flow_Cover_Cuts` 
     - FLOWCOVERCUTS
   * - :ref:`GUROBI_MIP_Cuts_-_Flow_Path_Cuts` 
     - FLOWPATHCUTS
   * - :ref:`GUROBI_MIP_Cuts_-_Global_Cut_Control`  
     - CUTS
   * - :ref:`GUROBI_MIP_Cuts_-_Gomory_Cuts_Passes_L` 
     - GOMORYPASSES
   * - :ref:`GUROBI_MIP_Cuts_-_GUB_Cover_Cuts` 
     - GUBCOVERCUTS
   * - :ref:`GUROBI_MIP_Cuts_-_Implied_Bound_Cuts` 
     - IMPLIEDCUTS
   * - :ref:`GUROBI_MIP_Cuts_-_Infeasibility_Proof_Cuts` 
     - INFPROOFCUTS
   * - :ref:`GUROBI_MIP_Cuts_-_Lift_and_Project_Cuts`  
     - LIFTPROJECTCUTS
   * - :ref:`GUROBI_MIP_Cuts_-_MIP_Separation_Cuts`  
     - MIPSEPCUTS
   * - :ref:`GUROBI_MIP_Cuts_-_MIR_Cuts`  
     - MIRCUTS
   * - :ref:`GUROBI_MIP_Cuts_-_Mixing_Cuts`  
     - MIXINGCUTS
   * - :ref:`GUROBI_MIP_Cuts_-_Mod_K_cuts`  
     - MODKCUTS
   * - :ref:`GUROBI_MIP_Cuts_-_Network_Cuts`  
     - NETWORKCUTS
   * - :ref:`GUROBI_MIP_Cuts_-_Projected_Implied_Bound_Cuts` 
     - PROJIMPLIEDCUTS
   * - :ref:`GUROBI_MIP_Cuts_-_Relax-and-lift_Cuts`  
     - RELAXLIFTCUTS
   * - :ref:`GUROBI_MIP_Cuts_-_RLT_Cuts` 
     - RLTCUTS
   * - :ref:`GUROBI_MIP_Cuts_-_Root_Cut_Passes_Limit` 
     - CUTPASSES
   * - :ref:`GUROBI_MIP_Cuts_-_Strong_CG_Cuts`  
     - STRONGCGCUTS
   * - :ref:`GUROBI_MIP_Cuts_-_Sub_MIP_Cuts`  
     - SUBMIPCUTS
   * - :ref:`GUROBI_MIP_Cuts_-_Zero_Half_Cuts`  
     - ZEROHALFCUTS
   * - :ref:`GUROBI_MIP_Heuristic_-_Feasibility_Pump_Passes` 
     - PUMPPASSES
   * - :ref:`GUROBI_MIP_Heuristic_-_Heuristics`  
     - HEURISTICS
   * - :ref:`GUROBI_MIP_Heuristic_-_Minimum_Relaxation_Heuristic_N` 
     - MINRELNODES
   * - :ref:`GUROBI_MIP_Heuristic_-_No_Relaxation_Heuristic_Time` 
     - NORELHEURTIME
   * - :ref:`GUROBI_MIP_Heuristic_-_No_Relaxation_Heuristic_Work` 
     - NORELHEURWORK
   * - :ref:`GUROBI_MIP_Heuristic_-_Partition_Heuristic`  
     - PARTITIONPLACE
   * - :ref:`GUROBI_MIP_Heuristic_-_RINS_Heuristic_Frequency`  
     - RINS
   * - :ref:`GUROBI_MIP_Heuristic_-_RINS_Sub_Node_Lim`  
     - SUBMIPNODES
   * - :ref:`GUROBI_MIP_Heuristic_-_Zero_Objective_Node_Limit` 
     - ZEROOBJNODES
   * - :ref:`GUROBI_MIP_Presolve_-_MIP_OBBT` 
     - OBBT
   * - :ref:`GUROBI_MIP_Presolve_-_Presolve_Sparsify_Reduction` 
     - PRESPARSIFY
   * - :ref:`GUROBI_MIP_Presolve_-_SOS1_Encoding` 
     - PRESOS1ENCODING
   * - :ref:`GUROBI_MIP_Presolve_-_SOS1_Reformulation_Threshold` 
     - PRESOS1BIGM
   * - :ref:`GUROBI_MIP_Presolve_-_SOS2_Encoding` 
     - PRESOS2ENCODING
   * - :ref:`GUROBI_MIP_Presolve_-_SOS2_Reformulation_Threshold` 
     - PRESOS2BIGM
   * - :ref:`GUROBI_Nonlinear_-_Maximal_Variable_Bound` 
     - 
   * - :ref:`GUROBI_Nonlinear_-_Nonlinear_Optimality_Tol` 
     - MIPGAP
   * - :ref:`GUROBI_Parallel_-_Concurrent_MIP` 
     - CONCURRENTMIP
   * - :ref:`GUROBI_Parallel_-_Thread_Limit` 
     - THREADS
   * - :ref:`GUROBI_Presolve_-_Dual_Reductions` 
     - DUALREDUCTIONS
   * - :ref:`GUROBI_Presolve_-_Linearize_Quadratic_Constraint` 
     - PREQLINEARIZE
   * - :ref:`GUROBI_Presolve_-_Multi_Objective_Presolve`  
     - MULTIOBJPRE
   * - :ref:`GUROBI_Presolve_-_Presolve` 
     - PRESOLVE
   * - :ref:`GUROBI_Presolve_-_Presolve_Aggregation`  
     - AGGREGATE
   * - :ref:`GUROBI_Presolve_-_Presolve_Aggregation_Fill`  
     - AGGFILL
   * - :ref:`GUROBI_Presolve_-_Presolve_Dual` 
     - PREDUAL
   * - :ref:`GUROBI_Presolve_-_Presolve_Passes` 
     - PREPASSES
   * - :ref:`GUROBI_Presolve_-_Presolve_Row_Reduction` 
     - PREDEPROW
   * - :ref:`GUROBI_Quadratic_-_MIQCP_Formulation` 
     - PREMIQCPFORM
   * - :ref:`GUROBI_Quadratic_-_MIQCP_Method` 
     - MIQCPMETHOD
   * - :ref:`GUROBI_Quadratic_-_NLP_Heuristic` 
     - NLPHEUR
   * - :ref:`GUROBI_Quadratic_-_Nonconvex_Strategy` 
     - NONCONVEX
   * - :ref:`GUROBI_Quadratic_-_PSD_Tolerance` 
     - PSDTOL
   * - :ref:`GUROBI_Quadratic_-_QCP_Dual_Values` 
     - QCPDUAL
   * - :ref:`GUROBI_Simplex_-_Degenerate_Simplex_Moves_Limit` 
     - DEGENMOVES
   * - :ref:`GUROBI_Simplex_-_Markowitz` 
     - MARKOWITZTOL	
   * - :ref:`GUROBI_Simplex_-_Network_Algorithm` 
     - NETWORKALG
   * - :ref:`GUROBI_Simplex_-_Norm_Adjust` 
     - NORMADJUST
   * - :ref:`GUROBI_Simplex_-_Objective_Scale` 
     - OBJSCALE
   * - :ref:`GUROBI_Simplex_-_Perturbation` 
     - PERTURBVALUE
   * - :ref:`GUROBI_Simplex_-_Pricing`  
     - SIMPLEXPRICING
   * - :ref:`GUROBI_Simplex_-_Quad_Precision`  
     - QUAD
   * - :ref:`GUROBI_Simplex_-_Sifting` 
     - SIFTING
   * - :ref:`GUROBI_Simplex_-_Sifting_Method` 
     - SIFTMETHOD
   * - :ref:`GUROBI_Solution_Pool_-_Pool_Absolute_Gap` 
     - POOLGAPABS
   * - :ref:`GUROBI_Solution_Pool_-_Pool_Gap` 
     - POOLGAP
   * - :ref:`GUROBI_Solution_Pool_-_Pool_Search_Mode` 
     - POOLSEARCHMODE
   * - :ref:`GUROBI_Solution_Pool_-_Pool_Size` 
     - POOLSOLUTIONS
   * - :ref:`GUROBI_Tuning_-_Tune_Cleanup` 
     - TUNECLEANUP
   * - :ref:`GUROBI_Tuning_-_Tune_Criterion` 
     - TUNECRITERION
   * - :ref:`GUROBI_Tuning_-_Tune_Metric` 
     - TUNEMETRIC
   * - :ref:`GUROBI_Tuning_-_Tune_Results` 
     - TUNERESULTS
   * - :ref:`GUROBI_Tuning_-_Tune_Target_MIP_Gap` 
     - TUNETARGETMIPGAP
   * - :ref:`GUROBI_Tuning_-_Tune_Target_Time` 
     - TUNETARGETTIME
   * - :ref:`GUROBI_Tuning_-_Tune_Time_Limit` 
     - TUNETIMELIMIT
   * - :ref:`GUROBI_Tuning_-_Tune_Trials`  
     - TUNETRIALS


				



The table below shows Solvers General options that are mapped to Gurobi parameters.




.. list-table::

   * - **Option name in AIMMS** 
     - **Name in GUROBI** 
   * - :ref:`Options_MIP_Options_-_Cutoff` 
     - CUTOFF
   * - :ref:`Options_MIP_Options_-_Maximal_Number_o` 
     - SOLUTIONLIMIT
   * - :ref:`Options_MIP_Options_-_MIP_Absolute_Opt` 
     - MIPGAPABS
   * - :ref:`Options_MIP_Options_-_MIP_Relative_Opt` 
     - MIPGAP
   * - :ref:`Options_Stop_Criteria_-_Iteration_Limi` 
     - ITERATIONLIMIT
   * - :ref:`Options_Stop_Criteria_-_Time_Limit` 
     - TIMELIMIT


