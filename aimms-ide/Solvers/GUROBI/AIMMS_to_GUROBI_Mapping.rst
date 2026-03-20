

.. _AIMMS_to_GUROBI_Mapping:


AIMMS to Gurobi Mapping
============================

**Description** 

The table shows in the left column the AIMMS Gurobi options while the right column displays the associated Gurobi parameter.

.. list-table::

   * - **Option name in AIMMS** 
     - **Name in Gurobi** 
   * - :doc:`Barrier - Barrier Convergence Tolerance <Barrier/GUROBI_Barrier_-_Barrier_Convergence_Tolerance>`
     - BARCONVTOL
   * - :doc:`Barrier - Barrier Correction Steps <Barrier/GUROBI_Barrier_-_Barrier_Correction_Steps>`
     - BARCORRECTORS
   * - :doc:`Barrier - Barrier Crossover <Barrier/GUROBI_Barrier_-_Barrier_Crossover>`
     - CROSSOVER
   * - :doc:`Barrier - Barrier Crossover Basis <Barrier/GUROBI_Barrier_-_Barrier_Crossover_Basis>`
     - CROSSOVERBASIS
   * - :doc:`Barrier - Barrier Homogeneous Algorithm <Barrier/GUROBI_Barrier_-_Barrier_Homogeneous_Aalgorithm>`
     - BARHOMOGENEOUS
   * - :doc:`Barrier - Barrier Iteration Limit <Barrier/GUROBI_Barrier_-_Barrier_Iteration_Limit>`
     - BARITERLIMIT
   * - :doc:`Barrier - Barrier Ordering <Barrier/GUROBI_Barrier_-_Barrier_Ordering>`
     - BARORDER
   * - :doc:`Barrier - Barrier Progress Solution <Barrier/GUROBI_Barrier_-_Barrier_Progress_Solution>`
     - 
   * - :doc:`Barrier - Barrier QCP Convergence Tolerance <Barrier/GUROBI_Barrier_-_Barrier_QCP_Convergence_Tol>`
     - BARQCPCONVTOL
   * - :doc:`General - Calculate Kappa <General/GUROBI_General_-_Calculate_Kappa>`
     - 
   * - :doc:`General - Concurrent Method <General/GUROBI_General_-_Concurrent_Method>`
     - CONCURRENTMETHOD
   * - :doc:`General - Farkas Infeasibility Proof <General/GUROBI_General_-_Farkas_Infeasibility_Proof>`
     - 
   * - :doc:`General - Feasibility Tolerance <General/GUROBI_General_-_Feasibility>`
     - FEASIBILITYTOL
   * - :doc:`General - IIS Method <General/GUROBI_General_-_IIS_Method>`
     - FEASRELAXBIGM
   * - :doc:`General - IIS Method <General/GUROBI_General_-_IIS_Method>`
     - IISMETHOD
   * - :doc:`General - Memory Limit <General/GUROBI_General_-_Memory_Limit>`
     - MEMLIMIT
   * - :doc:`General - Method <General/GUROBI_General_-_Method>`
     - METHOD
   * - :doc:`General - MPS <General/GUROBI_General_-_MPS>`
     - 
   * - :doc:`General - MPS Dual <General/GUROBI_General_-_MPS_Dual>`
     - 
   * - :doc:`General - Multi-objective Method <General/GUROBI_General_-_Multi_objective_method>`
     - MULTIOBJMETHOD
   * - :doc:`General - Numeric Focus <General/GUROBI_General_-_Numeric_Focus>`
     - NUMERICFOCUS
   * - :doc:`General - Optimality Tolerance <General/GUROBI_General_-_Optimality>`
     - OPTIMALITYTOL
   * - :doc:`General - Random Seed <General/GUROBI_General_-_Random_Seed>`
     - SEED
   * - :doc:`General - Read Parameter File <General/GUROBI_General_-_Read_Parameter_File>`
     - 
   * - :doc:`General - Restart <General/GUROBI_General_-_Restart>`
     - 
   * - :doc:`General - Restart File Number <General/GUROBI_General_-_Restart_File_Nr>`
     - 
   * - :doc:`General - Scale <General/GUROBI_General_-_Scale>`
     - SCALEFLAG
   * - :doc:`General - Sensitivity Method <General/GUROBI_General_-_Sensitivity_Method>`
     - 
   * - :doc:`General - Soft Memory Limit <General/GUROBI_General_-_Soft_Memory_Limit>`
     - SOFTMEMLIMIT
   * - :doc:`General - Solution File <General/GUROBI_General_-_Solution_File>`
     - 
   * - :doc:`General - Solution Target <General/GUROBI_General_-_Solution_Target>`
     - SOLUTIONTARGET
   * - :doc:`General - Unbounded Ray <General/GUROBI_General_-_Unbounded_ray>`
     - 
   * - :doc:`General - Updates Batch Size <General/GUROBI_General_-_Updates_Batch_Size>`
     - 
   * - :doc:`General - Warm Start <General/GUROBI_General_-_Warm_Start>`
     - LPWARMSTART
   * - :doc:`General - Work Limit <General/GUROBI_General_-_Work_Limit>`
     - WORKLIMIT
   * - :doc:`General - Write Parameter File <General/GUROBI_General_-_Write_Parameter_File>`
     - 
   * - :doc:`Logging - Display Solution Quality <Logging/GUROBI_Logging_-_Display_Solution_Quality>`
     - 
   * - :doc:`Logging - Log to Console <Logging/GUROBI_Logging_-_Log_to_Console>`
     - LOGTOCONSOLE
   * - :doc:`Logging - Output File <Logging/GUROBI_Logging_-_Output_File>`
     - OUTPUTFLAG
   * - :doc:`Logging - Output File Display Interval <Logging/GUROBI_Logging_-_Output_File_Display_Interval>`
     - DISPLAYINTERVAL
   * - :doc:`Logging - Tune Output Level <Logging/GUROBI_Logging_-_Tune_Output_Level>`
     - TUNEOUTPUT
   * - :doc:`MIP - Branch Direction <MIP/GUROBI_MIP_-_Branch_direction>`
     - BRANCHDIR
   * - :doc:`MIP - Disconnected Component Strategy <MIP/GUROBI_MIP_-_Disconnected_Component_Strateg>`
     - DISCONNECTED
   * - :doc:`MIP - Hints File <MIP/GUROBI_MIP_-_Hints_File>`
     - 
   * - :doc:`MIP - Improve Start Gap <MIP/GUROBI_MIP_-_Improve_Start_Gap>`
     - IMPROVESTARTGAP
   * - :doc:`MIP - Improve Start Nodes <MIP/GUROBI_MIP_-_Improve_Start_Nodes>`
     - IMPROVESTARTNODES
   * - :doc:`MIP - Improve Start Time <MIP/GUROBI_MIP_-_Improve_Start_Time>`
     - IMPROVESTARTTIME
   * - :doc:`MIP - Improve Start Work <MIP/GUROBI_MIP_-_Improve_Start_Work>`
     - IMPROVESTARTWORK
   * - :doc:`MIP - Integrality Tolerance <MIP/GUROBI_MIP_-_Integrality>`
     - INTFEASTOL
   * - :doc:`MIP - Integrality Focus <MIP/GUROBI_MIP_-_Integrality_Focus>`
     - INTEGRALITYFOCUS
   * - :doc:`MIP - Lazy Constraint Mode <MIP/GUROBI_MIP_-_Lazy_Constraint_Mode>`
     - 
   * - :doc:`MIP - MIP Best Bound Stop <MIP/GUROBI_MIP_-_MIP_Best_Bound_Stop>`
     - BESTBDSTOP
   * - :doc:`MIP - MIP Best Objective Stop <MIP/GUROBI_MIP_-_MIP_Best_Objective_Stop>`
     - BESTOBJSTOP
   * - :doc:`MIP - MIP Focus <MIP/GUROBI_MIP_-_MIP_Focus>`
     - MIPFOCUS
   * - :doc:`MIP - MIP Node Method <MIP/GUROBI_MIP_-_MIP_Node_Method>`
     - NODEMETHOD
   * - :doc:`MIP - MIP Start <MIP/GUROBI_MIP_-_MIP_Start>`
     - 
   * - :doc:`MIP - MIP Start Node Limit <MIP/GUROBI_MIP_-_MIP_Start_Node_Limit>`
     - STARTNODELIMIT
   * - :doc:`MIP - MIP Start Time Limit <MIP/GUROBI_MIP_-_MIP_Start_Time_Limit>`
     - STARTTIMELIMIT
   * - :doc:`MIP - MIP Start Work Limit <MIP/GUROBI_MIP_-_MIP_Start_Work_Limit>`
     - STARTWORKLIMIT
   * - :doc:`MIP - MIP Symmetry <MIP/GUROBI_MIP_-_MIP_Symmetry>`
     - SYMMETRY
   * - :doc:`MIP - Node File Start <MIP/GUROBI_MIP_-_Node_File_Start>`
     - NODEFILESTART
   * - :doc:`MIP - Node Limit <MIP/GUROBI_MIP_-_Node_Limit>`
     - NODELIMIT
   * - :doc:`MIP - Select Variables <MIP/GUROBI_MIP_-_Select_Variables>`
     - VARBRANCH
   * - :doc:`MIP Cuts - BQP Cuts <MIP Cuts/GUROBI_MIP_Cuts_-_BQP_Cuts>`
     - BQPCUTS
   * - :doc:`MIP Cuts - Clique Cuts <MIP Cuts/GUROBI_MIP_Cuts_-_Clique_Cuts>`
     - CLIQUECUTS
   * - :doc:`MIP Cuts - Cover Cuts <MIP Cuts/GUROBI_MIP_Cuts_-_Cover_Cuts>`
     - COVERCUTS
   * - :doc:`MIP Cuts - Dual Implied Cuts <MIP Cuts/GUROBI_MIP_Cuts_-_Dual_Implied_Cuts>`
     - DUALIMPLIEDCUTS
   * - :doc:`MIP Cuts - Cut Aggregation Passes Limit <MIP Cuts/GUROBI_MIP_Cuts_-_Cut_Aggr_Passes_Limit>`
     - CUTAGGPASSES
   * - :doc:`MIP Cuts - Flow Cover Cuts <MIP Cuts/GUROBI_MIP_Cuts_-_Flow_Cover_Cuts>`
     - FLOWCOVERCUTS
   * - :doc:`MIP Cuts - Flow Path Cuts <MIP Cuts/GUROBI_MIP_Cuts_-_Flow_Path_Cuts>`
     - FLOWPATHCUTS
   * - :doc:`MIP Cuts - Global Cut Control <MIP Cuts/GUROBI_MIP_Cuts_-_Global_Cut_Control>`
     - CUTS
   * - :doc:`MIP Cuts - Gomory Cut Passes Limit <MIP Cuts/GUROBI_MIP_Cuts_-_Gomory_Cuts_Passes_L>`
     - GOMORYPASSES
   * - :doc:`MIP Cuts - GUB Cover Cuts <MIP Cuts/GUROBI_MIP_Cuts_-_GUB_Cover_Cuts>`
     - GUBCOVERCUTS
   * - :doc:`MIP Cuts - Implied Bound Cuts <MIP Cuts/GUROBI_MIP_Cuts_-_Implied_Bound_Cuts>`
     - IMPLIEDCUTS
   * - :doc:`MIP Cuts - Infeasibility Proof Cuts <MIP Cuts/GUROBI_MIP_Cuts_-_Infeasibility_Proof_Cuts>`
     - INFPROOFCUTS
   * - :doc:`MIP Cuts - Lift and Project Cuts <MIP Cuts/GUROBI_MIP_Cuts_-_Lift_and_Project_Cuts>`
     - LIFTPROJECTCUTS
   * - :doc:`MIP Cuts - Master Knapsack Cuts <MIP Cuts/GUROBI_MIP_Cuts_-_Master_Knapsack_Cuts>`
     - MASTERKNAPSACKCUTS
   * - :doc:`MIP Cuts - MIP Separation Cuts <MIP Cuts/GUROBI_MIP_Cuts_-_MIP_Separation_Cuts>`
     - MIPSEPCUTS
   * - :doc:`MIP Cuts - MIR Cuts <MIP Cuts/GUROBI_MIP_Cuts_-_MIR_Cuts>`
     - MIRCUTS
   * - :doc:`MIP Cuts - Mixing Cuts <MIP Cuts/GUROBI_MIP_Cuts_-_Mixing_Cuts>`
     - MIXINGCUTS
   * - :doc:`MIP Cuts - Mod K Cuts <MIP Cuts/GUROBI_MIP_Cuts_-_Mod_K_cuts>`
     - MODKCUTS
   * - :doc:`MIP Cuts - Network Cuts <MIP Cuts/GUROBI_MIP_Cuts_-_Network_Cuts>`
     - NETWORKCUTS
   * - :doc:`MIP Cuts - Projected Implied Bound Cuts <MIP Cuts/GUROBI_MIP_Cuts_-_Projected_Implied_Bound_Cuts>`
     - PROJIMPLIEDCUTS
   * - :doc:`MIP Cuts - Relax-and-Lift Cuts <MIP Cuts/GUROBI_MIP_Cuts_-_Relax-and-lift_Cuts>`
     - RELAXLIFTCUTS
   * - :doc:`MIP Cuts - RLT Cuts <MIP Cuts/GUROBI_MIP_Cuts_-_RLT_Cuts>`
     - RLTCUTS
   * - :doc:`MIP Cuts - Root Cut Passes Limit <MIP Cuts/GUROBI_MIP_Cuts_-_Root_Cut_Passes_Limit>`
     - CUTPASSES
   * - :doc:`MIP Cuts - Strong CG Cuts <MIP Cuts/GUROBI_MIP_Cuts_-_Strong_CG_Cuts>`
     - STRONGCGCUTS
   * - :doc:`MIP Cuts - Sub MIP Cuts <MIP Cuts/GUROBI_MIP_Cuts_-_Sub_MIP_Cuts>`
     - SUBMIPCUTS
   * - :doc:`MIP Cuts - Zero Half Cuts <MIP Cuts/GUROBI_MIP_Cuts_-_Zero_Half_Cuts>`
     - ZEROHALFCUTS
   * - :doc:`MIP Heuristics - Feasibility Pump Passes <MIP Heuristics/GUROBI_MIP_Heuristic_-_Feasibility_Pump_Passes>`
     - PUMPPASSES
   * - :doc:`MIP Heuristics - Heuristics <MIP Heuristics/GUROBI_MIP_Heuristic_-_Heuristics>`
     - HEURISTICS
   * - :doc:`MIP Heuristics - Minimum Relaxation Heuristic Node Limit <MIP Heuristics/GUROBI_MIP_Heuristic_-_Minimum_Relaxation_Heuristic_N>`
     - MINRELNODES
   * - :doc:`MIP Heuristics - No Relaxation Heuristic Limit <MIP Heuristics/GUROBI_MIP_Heuristic_-_No_Relaxation_Heuristic_Limit>`
     - NORELHEURSOLUTIONS
   * - :doc:`MIP Heuristics - No Relaxation Heuristic Time <MIP Heuristics/GUROBI_MIP_Heuristic_-_No_Relaxation_Heuristic_Time>`
     - NORELHEURTIME
   * - :doc:`MIP Heuristics - No Relaxation Heuristic Work <MIP Heuristics/GUROBI_MIP_Heuristic_-_No_Relaxation_Heuristic_Work>`
     - NORELHEURWORK
   * - :doc:`MIP Heuristics - Partition Heuristic <MIP Heuristics/GUROBI_MIP_Heuristic_-_Partition_Heuristic>`
     - PARTITIONPLACE
   * - :doc:`MIP Heuristics - RINS Heuristic Frequency <MIP Heuristics/GUROBI_MIP_Heuristic_-_RINS_Heuristic_Frequency>`
     - RINS
   * - :doc:`MIP Heuristics - RINS Sub-MIP Node Limit <MIP Heuristics/GUROBI_MIP_Heuristic_-_RINS_Sub_Node_Lim>`
     - SUBMIPNODES
   * - :doc:`MIP Heuristics - Zero Objective Node Limit <MIP Heuristics/GUROBI_MIP_Heuristic_-_Zero_Objective_Node_Limit>`
     - ZEROOBJNODES
   * - :doc:`MIP Presolve - MIP OBBT <MIP Presolve/GUROBI_MIP_Presolve_-_MIP_OBBT>`
     - OBBT
   * - :doc:`MIP Presolve - Presolve Sparsify Reduction <MIP Presolve/GUROBI_MIP_Presolve_-_Presolve_Sparsify_Reduction>`
     - PRESPARSIFY
   * - :doc:`MIP Presolve - SOS1 Encoding <MIP Presolve/GUROBI_MIP_Presolve_-_SOS1_Encoding>`
     - PRESOS1ENCODING
   * - :doc:`MIP Presolve - SOS1 Reformulation Threshold <MIP Presolve/GUROBI_MIP_Presolve_-_SOS1_Reformulation_Threshold>`
     - PRESOS1BIGM
   * - :doc:`MIP Presolve - SOS2 Encoding <MIP Presolve/GUROBI_MIP_Presolve_-_SOS2_Encoding>`
     - PRESOS2ENCODING
   * - :doc:`MIP Presolve - SOS2 Reformulation Threshold <MIP Presolve/GUROBI_MIP_Presolve_-_SOS2_Reformulation_Threshold>`
     - PRESOS2BIGM
   * - :doc:`Nonlinear - Maximal Variable Bound <Nonlinear/GUROBI_Nonlinear_-_Maximal_Variable_Bound>`
     - 
   * - :doc:`Nonlinear - NLP Heuristic <Nonlinear/GUROBI_Nonlinear_-_NLP_Heuristic>`
     - NLPHEUR
   * - :doc:`Nonlinear - Nonlinear Optimality Tolerance <Nonlinear/GUROBI_Nonlinear_-_Nonlinear_Optimality_Tol>`
     - MIPGAP
   * - :doc:`Parallel - Concurrent MIP <Parallel/GUROBI_Parallel_-_Concurrent_MIP>`
     - CONCURRENTMIP
   * - :doc:`Parallel - Thread Limit <Parallel/GUROBI_Parallel_-_Thread_Limit>`
     - THREADS
   * - :doc:`PDHG - PDHG Absolute Feasibility Tolerance <PDHG/GUROBI_PDHG_-_PDHG_Absolute_Feasibility_Tol>`
     - PDHGABSTOL
   * - :doc:`PDHG - PDHG Convergence Tolerance <PDHG/GUROBI_PDHG_-_PDHG_Convergence_Tol>`
     - PDHGCONVTOL
   * - :doc:`PDHG - PDHG Iteration Limit <PDHG/GUROBI_PDHG_-_PDHG_Iteration_Limit>`
     - PDHGITERLIMIT
   * - :doc:`PDHG - PDHG Relative Feasibility Tolerance <PDHG/GUROBI_PDHG_-_PDHG_Relative_Feasibility_Tol>`
     - PDHGRELTOL
   * - :doc:`Presolve - Dual Reductions <Presolve/GUROBI_Presolve_-_Dual_Reductions>`
     - DUALREDUCTIONS
   * - :doc:`Presolve - Linearize Quadratic Constraints <Presolve/GUROBI_Presolve_-_Linearize_Quadratic_Constraint>`
     - PREQLINEARIZE
   * - :doc:`Presolve - Multi-objective Presolve <Presolve/GUROBI_Presolve_-_Multi_Objective_Presolve>`
     - MULTIOBJPRE
   * - :doc:`Presolve - Presolve <Presolve/GUROBI_Presolve_-_Presolve>`
     - PRESOLVE
   * - :doc:`Presolve - Presolve Aggregation <Presolve/GUROBI_Presolve_-_Presolve_Aggregation>`
     - AGGREGATE
   * - :doc:`Presolve - Presolve Aggregation Fill <Presolve/GUROBI_Presolve_-_Presolve_Aggregation_Fill>`
     - AGGFILL
   * - :doc:`Presolve - Presolve Dual <Presolve/GUROBI_Presolve_-_Presolve_Dual>`
     - PREDUAL
   * - :doc:`Presolve - Presolve Passes <Presolve/GUROBI_Presolve_-_Presolve_Passes>`
     - PREPASSES
   * - :doc:`Presolve - Presolve Row Reduction <Presolve/GUROBI_Presolve_-_Presolve_Row_Reduction>`
     - PREDEPROW
   * - :doc:`Quadratic - MIQCP Formulation <Quadratic/GUROBI_Quadratic_-_MIQCP_Formulation>`
     - PREMIQCPFORM
   * - :doc:`Quadratic - MIQCP Method <Quadratic/GUROBI_Quadratic_-_MIQCP_Method>`
     - MIQCPMETHOD
   * - :doc:`Quadratic - Nonconvex Strategy <Quadratic/GUROBI_Quadratic_-_Nonconvex_Strategy>`
     - NONCONVEX
   * - :doc:`Quadratic - PSD Tolerance <Quadratic/GUROBI_Quadratic_-_PSD_Tolerance>`
     - PSDTOL
   * - :doc:`Quadratic - QCP Dual Values <Quadratic/GUROBI_Quadratic_-_QCP_Dual_Values>`
     - QCPDUAL
   * - :doc:`Simplex - Degenerate Simplex Moves Limit <Simplex/GUROBI_Simplex_-_Degenerate_Simplex_Moves_Limit>`
     - DEGENMOVES
   * - :doc:`Simplex - Markowitz Tolerance <Simplex/GUROBI_Simplex_-_Markowitz>`
     - MARKOWITZTOL
   * - :doc:`Simplex - Network Algorithm <Simplex/GUROBI_Simplex_-_Network_Algorithm>`
     - NETWORKALG
   * - :doc:`Simplex - Norm Adjust <Simplex/GUROBI_Simplex_-_Norm_Adjust>`
     - NORMADJUST
   * - :doc:`Simplex - Objective Scale <Simplex/GUROBI_Simplex_-_Objective_Scale>`
     - OBJSCALE
   * - :doc:`Simplex - Perturbation <Simplex/GUROBI_Simplex_-_Perturbation>`
     - PERTURBVALUE
   * - :doc:`Simplex - Pricing <Simplex/GUROBI_Simplex_-_Pricing>`
     - SIMPLEXPRICING
   * - :doc:`Simplex - Quad Precision <Simplex/GUROBI_Simplex_-_Quad_Precision>`
     - QUAD
   * - :doc:`Simplex - Sifting <Simplex/GUROBI_Simplex_-_Sifting>`
     - SIFTING
   * - :doc:`Simplex - Sifting Method <Simplex/GUROBI_Simplex_-_Sifting_Method>`
     - SIFTMETHOD
   * - :doc:`Solution Pool - Pool Absolute Gap <Solution Pool/GUROBI_Solution_Pool_-_Pool_Absolute_Gap>`
     - POOLGAPABS
   * - :doc:`Solution Pool - Pool Gap <Solution Pool/GUROBI_Solution_Pool_-_Pool_Gap>`
     - POOLGAP
   * - :doc:`Solution Pool - Pool Search Mode <Solution Pool/GUROBI_Solution_Pool_-_Pool_Search_Mode>`
     - POOLSEARCHMODE
   * - :doc:`Solution Pool - Pool Size <Solution Pool/GUROBI_Solution_Pool_-_Pool_Size>`
     - POOLSOLUTIONS
   * - :doc:`Tuning - Tune Cleanup <Tuning/GUROBI_Tuning_-_Tune_Cleanup>`
     - TUNECLEANUP
   * - :doc:`Tuning - Tune Criterion <Tuning/GUROBI_Tuning_-_Tune_Criterion>`
     - TUNECRITERION
   * - :doc:`Tuning - Tune Metric <Tuning/GUROBI_Tuning_-_Tune_Metric>`
     - TUNEMETRIC
   * - :doc:`Tuning - Tune Results <Tuning/GUROBI_Tuning_-_Tune_Results>`
     - TUNERESULTS
   * - :doc:`Tuning - Tune Target MIP Gap <Tuning/GUROBI_Tuning_-_Tune_Target_MIP_Gap>`
     - TUNETARGETMIPGAP
   * - :doc:`Tuning - Tune Target Time <Tuning/GUROBI_Tuning_-_Tune_Target_Time>`
     - TUNETARGETTIME
   * - :doc:`Tuning - Tune Time Limit <Tuning/GUROBI_Tuning_-_Tune_Time_Limit>`
     - TUNETIMELIMIT
   * - :doc:`Tuning - Tune Trials <Tuning/GUROBI_Tuning_-_Tune_Trials>`
     - TUNETRIALS


The table below shows Solvers General options that are mapped to Gurobi parameters.

.. list-table::

   * - **Option name in AIMMS** 
     - **Name in GUROBI** 
   * - :doc:`MIP Options - Cutoff <../../Aimms/Options/Solvers General/MIP Options/MIP_Options_-_Cutoff>`
     - CUTOFF
   * - :doc:`MIP Options - Maximal Number of Integer Solutions <../../Aimms/Options/Solvers General/MIP Options/MIP_Options_-_Maximal_Number_o>`
     - SOLUTIONLIMIT
   * - :doc:`MIP Options - MIP Absolute Optimality Tolerance <../../Aimms/Options/Solvers General/MIP Options/MIP_Options_-_MIP_Absolute_Opt>`
     - MIPGAPABS
   * - :doc:`MIP Options - MIP Relative Optimality Tolerance <../../Aimms/Options/Solvers General/MIP Options/MIP_Options_-_MIP_Relative_Opt>`
     - MIPGAP
   * - :doc:`Stop Criteria - Iteration Limit <../../Aimms/Options/Solvers General/Stop Criteria/Stop_Criteria_-_Iteration_Limi>`
     - ITERATIONLIMIT
   * - :doc:`Stop Criteria - Time Limit <../../Aimms/Options/Solvers General/Stop Criteria/Stop_Criteria_-_Time_Limit>`
     - TIMELIMIT



