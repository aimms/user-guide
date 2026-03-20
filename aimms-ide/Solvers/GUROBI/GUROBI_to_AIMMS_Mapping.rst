

.. _GUROBI_to_AIMMS_Mapping:


Gurobi to AIMMS Mapping
============================

**Description** 

The table shows in the left column the parameters from Gurobi that can be set in AIMMS; 
the right column displays for each Gurobi parameter the associated AIMMS option.

.. list-table::

   * - **Name in Gurobi**
     - **Option name in AIMMS**
   * - AGGFILL
     - :doc:`Presolve - Presolve Aggregation Fill <Presolve/GUROBI_Presolve_-_Presolve_Aggregation_Fill>`
   * - AGGREGATE
     - :doc:`Presolve - Presolve Aggregation <Presolve/GUROBI_Presolve_-_Presolve_Aggregation>`
   * - BARCONVTOL
     - :doc:`Barrier - Barrier Convergence Tolerance <Barrier/GUROBI_Barrier_-_Barrier_Convergence_Tolerance>`
   * - BARCORRECTORS
     - :doc:`Barrier - Barrier Correction Steps <Barrier/GUROBI_Barrier_-_Barrier_Correction_Steps>`
   * - BARHOMOGENEOUS
     - :doc:`Barrier - Barrier Homogeneous Algorithm <Barrier/GUROBI_Barrier_-_Barrier_Homogeneous_Aalgorithm>`
   * - BARITERLIMIT
     - :doc:`Barrier - Barrier Iteration Limit <Barrier/GUROBI_Barrier_-_Barrier_Iteration_Limit>`
   * - BARORDER
     - :doc:`Barrier - Barrier Ordering <Barrier/GUROBI_Barrier_-_Barrier_Ordering>`
   * - BARQCPCONVTOL
     - :doc:`Barrier - Barrier QCP Convergence Tolerance <Barrier/GUROBI_Barrier_-_Barrier_QCP_Convergence_Tol>`
   * - BESTBDSTOP
     - :doc:`MIP - MIP Best Bound Stop <MIP/GUROBI_MIP_-_MIP_Best_Bound_Stop>`
   * - BESTOBJSTOP
     - :doc:`MIP - MIP Best Objective Stop <MIP/GUROBI_MIP_-_MIP_Best_Objective_Stop>`
   * - BQPCUTS
     - :doc:`MIP Cuts - BQP Cuts <MIP Cuts/GUROBI_MIP_Cuts_-_BQP_Cuts>`
   * - BRANCHDIR
     - :doc:`MIP - Branch Direction <MIP/GUROBI_MIP_-_Branch_direction>`
   * - CLIQUECUTS
     - :doc:`MIP Cuts - Clique Cuts <MIP Cuts/GUROBI_MIP_Cuts_-_Clique_Cuts>`
   * - CONCURRENTMETHOD
     - :doc:`General - Concurrent Method <General/GUROBI_General_-_Concurrent_Method>`
   * - CONCURRENTMIP
     - :doc:`Parallel - Concurrent MIP <Parallel/GUROBI_Parallel_-_Concurrent_MIP>`
   * - COVERCUTS
     - :doc:`MIP Cuts - Cover Cuts <MIP Cuts/GUROBI_MIP_Cuts_-_Cover_Cuts>`
   * - CROSSOVER
     - :doc:`Barrier - Barrier Crossover <Barrier/GUROBI_Barrier_-_Barrier_Crossover>`
   * - CROSSOVERBASIS
     - :doc:`Barrier - Barrier Crossover Basis <Barrier/GUROBI_Barrier_-_Barrier_Crossover_Basis>`
   * - CUTAGGPASSES
     - :doc:`MIP Cuts - Cut Aggregation Passes Limit <MIP Cuts/GUROBI_MIP_Cuts_-_Cut_Aggr_Passes_Limit>`
   * - CUTPASSES
     - :doc:`MIP Cuts - Root Cut Passes Limit <MIP Cuts/GUROBI_MIP_Cuts_-_Root_Cut_Passes_Limit>`
   * - CUTS
     - :doc:`MIP Cuts - Global Cut Control <MIP Cuts/GUROBI_MIP_Cuts_-_Global_Cut_Control>`
   * - DEGENMOVES
     - :doc:`Simplex - Degenerate Simplex Moves Limit <Simplex/GUROBI_Simplex_-_Degenerate_Simplex_Moves_Limit>`
   * - DISCONNECTED
     - :doc:`MIP - Disconnected Component Strategy <MIP/GUROBI_MIP_-_Disconnected_Component_Strateg>`
   * - DISPLAYINTERVAL
     - :doc:`Logging - Output File Display Interval <Logging/GUROBI_Logging_-_Output_File_Display_Interval>`
   * - DUALIMPLIEDCUTS
     - :doc:`MIP Cuts - Dual Implied Cuts <MIP Cuts/GUROBI_MIP_Cuts_-_Dual_Implied_Cuts>`
   * - DUALREDUCTIONS
     - :doc:`Presolve - Dual Reductions <Presolve/GUROBI_Presolve_-_Dual_Reductions>`
   * - FEASIBILITYTOL
     - :doc:`General - Feasibility Tolerance <General/GUROBI_General_-_Feasibility>`
   * - FEASRELAXBIGM
     - :doc:`General - FeasRelax Big M <General/GUROBI_General_-_FeasRelax_big-M>`
   * - FLOWCOVERCUTS
     - :doc:`MIP Cuts - Flow Cover Cuts <MIP Cuts/GUROBI_MIP_Cuts_-_Flow_Cover_Cuts>`
   * - FLOWPATHCUTS
     - :doc:`MIP Cuts - Flow Path Cuts <MIP Cuts/GUROBI_MIP_Cuts_-_Flow_Path_Cuts>`
   * - GOMORYPASSES
     - :doc:`MIP Cuts - Gomory Cut Passes Limit <MIP Cuts/GUROBI_MIP_Cuts_-_Gomory_Cuts_Passes_L>`
   * - GUBCOVERCUTS
     - :doc:`MIP Cuts - GUB Cover Cuts <MIP Cuts/GUROBI_MIP_Cuts_-_GUB_Cover_Cuts>`
   * - HEURISTICS
     - :doc:`MIP Heuristics - Heuristics <MIP Heuristics/GUROBI_MIP_Heuristic_-_Heuristics>`
   * - IISMETHOD
     - :doc:`General - IIS Method <General/GUROBI_General_-_IIS_Method>`
   * - IMPLIEDCUTS
     - :doc:`MIP Cuts - Implied Bound Cuts <MIP Cuts/GUROBI_MIP_Cuts_-_Implied_Bound_Cuts>`
   * - IMPROVESTARTGAP
     - :doc:`MIP - Improve Start Gap <MIP/GUROBI_MIP_-_Improve_Start_Gap>`
   * - IMPROVESTARTNODES
     - :doc:`MIP - Improve Start Nodes <MIP/GUROBI_MIP_-_Improve_Start_Nodes>`
   * - IMPROVESTARTTIME
     - :doc:`MIP - Improve Start Time <MIP/GUROBI_MIP_-_Improve_Start_Time>`
   * - IMPROVESTARTWORK
     - :doc:`MIP - Improve Start Work <MIP/GUROBI_MIP_-_Improve_Start_Work>`
   * - INFPROOFCUTS
     - :doc:`MIP Cuts - Infeasibility Proof Cuts <MIP Cuts/GUROBI_MIP_Cuts_-_Infeasibility_Proof_Cuts>`
   * - INTEGRALITYFOCUS
     - :doc:`MIP - Integrality Focus <MIP/GUROBI_MIP_-_Integrality_Focus>`
   * - INTFEASTOL
     - :doc:`MIP - Integrality Tolerance <MIP/GUROBI_MIP_-_Integrality>`
   * - LIFTPROJECTCUTS
     - :doc:`MIP Cuts - Lift and Project Cuts <MIP Cuts/GUROBI_MIP_Cuts_-_Lift_and_Project_Cuts>`
   * - LOGTOCONSOLE
     - :doc:`Logging - Log to Console <Logging/GUROBI_Logging_-_Log_to_Console>`
   * - LPWARMSTART
     - :doc:`General - Warm Start <General/GUROBI_General_-_Warm_Start>`
   * - MARKOWITZTOL
     - :doc:`Simplex - Markowitz Tolerance <Simplex/GUROBI_Simplex_-_Markowitz>`
   * - MASTERKNAPSACKCUTS
     - :doc:`MIP Cuts - Master Knapsack Cuts <MIP Cuts/GUROBI_MIP_Cuts_-_Master_Knapsack_Cuts>`
   * - MEMLIMIT
     - :doc:`General - Memory Limit <General/GUROBI_General_-_Memory_Limit>`
   * - METHOD
     - :doc:`General - Method <General/GUROBI_General_-_Method>`
   * - MINRELNODES
     - :doc:`MIP Heuristics - Minimum Relaxation Heuristic Node Limit <MIP Heuristics/GUROBI_MIP_Heuristic_-_Minimum_Relaxation_Heuristic_N>`
   * - MIPFOCUS
     - :doc:`MIP - MIP Focus <MIP/GUROBI_MIP_-_MIP_Focus>`
   * - MIPSEPCUTS
     - :doc:`MIP Cuts - MIP Separation Cuts <MIP Cuts/GUROBI_MIP_Cuts_-_MIP_Separation_Cuts>`
   * - MIQCPMETHOD
     - :doc:`Quadratic - MIQCP Method <Quadratic/GUROBI_Quadratic_-_MIQCP_Method>`
   * - MIRCUTS
     - :doc:`MIP Cuts - MIR Cuts <MIP Cuts/GUROBI_MIP_Cuts_-_MIR_Cuts>`
   * - MIXINGCUTS
     - :doc:`MIP Cuts - Mixing Cuts <MIP Cuts/GUROBI_MIP_Cuts_-_Mixing_Cuts>`
   * - MODKCUTS
     - :doc:`MIP Cuts - Mod K Cuts <MIP Cuts/GUROBI_MIP_Cuts_-_Mod_K_cuts>`
   * - MULTIOBJMETHOD
     - :doc:`General - Multi-objective Method <General/GUROBI_General_-_Multi_objective_method>`
   * - MULTIOBJPRE
     - :doc:`Presolve - Multi-objective Presolve <Presolve/GUROBI_Presolve_-_Multi_Objective_Presolve>`
   * - NETWORKALG
     - :doc:`Simplex - Network Algorithm <Simplex/GUROBI_Simplex_-_Network_Algorithm>`
   * - NETWORKCUTS
     - :doc:`MIP Cuts - Network Cuts <MIP Cuts/GUROBI_MIP_Cuts_-_Network_Cuts>`
   * - NLPHEUR
     - :doc:`Nonlinear - NLP Heuristic <Nonlinear/GUROBI_Nonlinear_-_NLP_Heuristic>`
   * - NODEFILESTART
     - :doc:`MIP - Node File Start <MIP/GUROBI_MIP_-_Node_File_Start>`
   * - NODELIMIT
     - :doc:`MIP - Node Limit <MIP/GUROBI_MIP_-_Node_Limit>`
   * - NODEMETHOD
     - :doc:`MIP - MIP Node Method <MIP/GUROBI_MIP_-_MIP_Node_Method>`
   * - NONCONVEX
     - :doc:`Quadratic - Nonconvex Strategy <Quadratic/GUROBI_Quadratic_-_Nonconvex_Strategy>`
   * - NORELHEURSOLUTIONS
     - :doc:`MIP Heuristics - No Relaxation Heuristic Limit <MIP Heuristics/GUROBI_MIP_Heuristic_-_No_Relaxation_Heuristic_Limit>`
   * - NORELHEURTIME
     - :doc:`MIP Heuristics - No Relaxation Heuristic Time <MIP Heuristics/GUROBI_MIP_Heuristic_-_No_Relaxation_Heuristic_Time>`
   * - NORELHEURWORK
     - :doc:`MIP Heuristics - No Relaxation Heuristic Work <MIP Heuristics/GUROBI_MIP_Heuristic_-_No_Relaxation_Heuristic_Work>`
   * - NORMADJUST
     - :doc:`Simplex - Norm Adjust <Simplex/GUROBI_Simplex_-_Norm_Adjust>`
   * - NUMERICFOCUS
     - :doc:`General - Numeric Focus <General/GUROBI_General_-_Numeric_Focus>`
   * - OBBT
     - :doc:`MIP Presolve - MIP OBBT <MIP Presolve/GUROBI_MIP_Presolve_-_MIP_OBBT>`
   * - OBJSCALE
     - :doc:`Simplex - Objective Scale <Simplex/GUROBI_Simplex_-_Objective_Scale>`
   * - OPTIMALITYTOL
     - :doc:`General - Optimality Tolerance <General/GUROBI_General_-_Optimality>`
   * - OUTPUTFLAG
     - :doc:`Logging - Output File <Logging/GUROBI_Logging_-_Output_File>`
   * - PARTITIONPLACE
     - :doc:`MIP Heuristics - Partition Heuristic <MIP Heuristics/GUROBI_MIP_Heuristic_-_Partition_Heuristic>`
   * - PDHGABSTOL
     - :doc:`PDHG - PDHG Absolute Feasibility Tolerance <PDHG/GUROBI_PDHG_-_PDHG_Absolute_Feasibility_Tol>`
   * - PDHGCONVTOL
     - :doc:`PDHG - PDHG Convergence Tolerance <PDHG/GUROBI_PDHG_-_PDHG_Convergence_Tol>`
   * - PDHGITERLIMIT
     - :doc:`PDHG - PDHG Iteration Limit <PDHG/GUROBI_PDHG_-_PDHG_Iteration_Limit>`
   * - PDHGRELTOL
     - :doc:`PDHG - PDHG Relative Feasibility Tolerance <PDHG/GUROBI_PDHG_-_PDHG_Relative_Feasibility_Tol>`
   * - PERTURBVALUE
     - :doc:`Simplex - Perturbation <Simplex/GUROBI_Simplex_-_Perturbation>`
   * - POOLGAP
     - :doc:`Solution Pool - Pool Gap <Solution Pool/GUROBI_Solution_Pool_-_Pool_Gap>`
   * - POOLGAPABS
     - :doc:`Solution Pool - Pool Absolute Gap <Solution Pool/GUROBI_Solution_Pool_-_Pool_Absolute_Gap>`
   * - POOLSEARCHMODE
     - :doc:`Solution Pool - Pool Search Mode <Solution Pool/GUROBI_Solution_Pool_-_Pool_Search_Mode>`
   * - POOLSOLUTIONS
     - :doc:`Solution Pool - Pool Size <Solution Pool/GUROBI_Solution_Pool_-_Pool_Size>`
   * - PREDEPROW
     - :doc:`Presolve - Presolve Row Reduction <Presolve/GUROBI_Presolve_-_Presolve_Row_Reduction>`
   * - PREDUAL
     - :doc:`Presolve - Presolve Dual <Presolve/GUROBI_Presolve_-_Presolve_Dual>`
   * - PREMIQCPFORM
     - :doc:`Quadratic - MIQCP Formulation <Quadratic/GUROBI_Quadratic_-_MIQCP_Formulation>`
   * - PREPASSES
     - :doc:`PPresolve - resolve Passes <Presolve/GUROBI_Presolve_-_Presolve_Passes>`
   * - PREQLINEARIZE
     - :doc:`Presolve - Linearize Quadratic Constraints <Presolve/GUROBI_Presolve_-_Linearize_Quadratic_Constraint>`
   * - PRESOLVE
     - :doc:`Presolve - Presolve <Presolve/GUROBI_Presolve_-_Presolve>`
   * - PRESOS1BIGM
     - :doc:`MIP Presolve - SOS1 Reformulation Threshold <MIP Presolve/GUROBI_MIP_Presolve_-_SOS1_Reformulation_Threshold>`
   * - PRESOS1ENCODING
     - :doc:`MIP Presolve - SOS1 Encoding <MIP Presolve/GUROBI_MIP_Presolve_-_SOS1_Encoding>`
   * - PRESOS2BIGM
     - :doc:`MIP Presolve - SOS2 Reformulation Threshold <MIP Presolve/GUROBI_MIP_Presolve_-_SOS2_Reformulation_Threshold>`
   * - PRESOS2ENCODING
     - :doc:`MIP Presolve - SOS2 Encoding <MIP Presolve/GUROBI_MIP_Presolve_-_SOS2_Encoding>`
   * - PRESPARSIFY
     - :doc:`MIP Presolve - Presolve Sparsify Reduction <MIP Presolve/GUROBI_MIP_Presolve_-_Presolve_Sparsify_Reduction>`
   * - PROJIMPLIEDCUTS
     - :doc:`MIP Cuts - Projected Implied Bound Cuts <MIP Cuts/GUROBI_MIP_Cuts_-_Projected_Implied_Bound_Cuts>`
   * - PSDTOL
     - :doc:`Quadratic - PSD Tolerance <Quadratic/GUROBI_Quadratic_-_PSD_Tolerance>`
   * - PUMPPASSES
     - :doc:`MIP Heuristics - Feasibility Pump Passes <MIP Heuristics/GUROBI_MIP_Heuristic_-_Feasibility_Pump_Passes>`
   * - QCPDUAL
     - :doc:`Quadratic - QCP Dual Values <Quadratic/GUROBI_Quadratic_-_QCP_Dual_Values>`
   * - QUAD
     - :doc:`Simplex - Quad Precision <Simplex/GUROBI_Simplex_-_Quad_Precision>`
   * - RELAXLIFTCUTS
     - :doc:`MIP Cuts - Relax-and-Lift Cuts <MIP Cuts/GUROBI_MIP_Cuts_-_Relax-and-lift_Cuts>`
   * - RINS
     - :doc:`MIP Heuristics - RINS Heuristic Frequency <MIP Heuristics/GUROBI_MIP_Heuristic_-_RINS_Heuristic_Frequency>`
   * - RLTCUTS
     - :doc:`MIP Cuts - RLT Cuts <MIP Cuts/GUROBI_MIP_Cuts_-_RLT_Cuts>`
   * - SCALEFLAG
     - :doc:`General - Scale <General/GUROBI_General_-_Scale>`
   * - SEED
     - :doc:`General - Random Seed <General/GUROBI_General_-_Random_Seed>`
   * - SIFTING
     - :doc:`Simplex - Sifting <Simplex/GUROBI_Simplex_-_Sifting>`
   * - SIFTMETHOD
     - :doc:`Simplex - Sifting Method <Simplex/GUROBI_Simplex_-_Sifting_Method>`
   * - SIMPLEXPRICING
     - :doc:`Simplex - Pricing <Simplex/GUROBI_Simplex_-_Pricing>`
   * - SOFTMEMLIMIT
     - :doc:`General - Soft Memory Limit <General/GUROBI_General_-_Soft_Memory_Limit>`
   * - SOLUTIONTARGET
     - :doc:`General - Solution Target <General/GUROBI_General_-_Solution_Target>`
   * - STARTNODELIMIT
     - :doc:`MIP - MIP Start Node Limit <MIP/GUROBI_MIP_-_MIP_Start_Node_Limit>`
   * - STARTTIMELIMIT
     - :doc:`MIP - MIP Start Time Limit <MIP/GUROBI_MIP_-_MIP_Start_Time_Limit>`
   * - STARTWORKLIMIT
     - :doc:`MIP - MIP Start Work Limit <MIP/GUROBI_MIP_-_MIP_Start_Work_Limit>`
   * - STRONGCGCUTS
     - :doc:`MIP Cuts - Strong CG Cuts <MIP Cuts/GUROBI_MIP_Cuts_-_Strong_CG_Cuts>`
   * - SUBMIPCUTS
     - :doc:`MIP Cuts - Sub MIP Cuts <MIP Cuts/GUROBI_MIP_Cuts_-_Sub_MIP_Cuts>`
   * - SUBMIPNODES
     - :doc:`MIP Heuristics - RINS Sub-MIP Node Limit <MIP Heuristics/GUROBI_MIP_Heuristic_-_RINS_Sub_Node_Lim>`
   * - SYMMETRY
     - :doc:`MIP - MIP Symmetry <MIP/GUROBI_MIP_-_MIP_Symmetry>`
   * - THREADS
     - :doc:`Parallel - Thread Limit <Parallel/GUROBI_Parallel_-_Thread_Limit>`
   * - TUNECLEANUP
     - :doc:`Tuning - Tune Cleanup <Tuning/GUROBI_Tuning_-_Tune_Cleanup>`
   * - TUNECRITERION
     - :doc:`Tuning - Tune Criterion <Tuning/GUROBI_Tuning_-_Tune_Criterion>`
   * - TUNEMETRIC
     - :doc:`Tuning - Tune Metric <Tuning/GUROBI_Tuning_-_Tune_Metric>`
   * - TUNEOUTPUT
     - :doc:`Logging - Tune Output Level <Logging/GUROBI_Logging_-_Tune_Output_Level>`
   * - TUNERESULTS
     - :doc:`Tuning - Tune Results <Tuning/GUROBI_Tuning_-_Tune_Results>`
   * - TUNETARGETMIPGAP
     - :doc:`Tuning - Tune Target MIP Gap <Tuning/GUROBI_Tuning_-_Tune_Target_MIP_Gap>`
   * - TUNETARGETTIME
     - :doc:`Tuning - Tune Target Time <Tuning/GUROBI_Tuning_-_Tune_Target_Time>`
   * - TUNETIMELIMIT
     - :doc:`Tuning - Tune Time Limit <Tuning/GUROBI_Tuning_-_Tune_Time_Limit>`
   * - TUNETRIALS
     - :doc:`Tuning - Tune Trials <Tuning/GUROBI_Tuning_-_Tune_Trials>`
   * - VARBRANCH
     - :doc:`MIP - Select Variables <MIP/GUROBI_MIP_-_Select_Variables>`
   * - WORKLIMIT
     - :doc:`General - Work Limit <General/GUROBI_General_-_Work_Limit>`
   * - ZEROHALFCUTS
     - :doc:`MIP Cuts - Zero Half Cuts <MIP Cuts/GUROBI_MIP_Cuts_-_Zero_Half_Cuts>`
   * - ZEROOBJNODES
     - :doc:`MIP Heuristics - Zero Objective Node Limit <MIP Heuristics/GUROBI_MIP_Heuristic_-_Zero_Objective_Node_Limit>`


**Note** 

*	The Gurobi parameter PRECRUSH is not available in AIMMS. AIMMS automatically switches it on when a cut callback procedure is installed in the AIMMS model.
