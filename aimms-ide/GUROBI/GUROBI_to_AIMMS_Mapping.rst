

.. _GUROBI_to_AIMMS_Mapping:
.. _GUROBI_GUROBI_to_AIMMS_Mapping:


GUROBI to AIMMS Mapping
============================

**Description** 

The table shows in the left column the parameters from Gurobi that can be set in AIMMS; 
the right column displays for each Gurobi parameter the associated AIMMS option.

.. list-table::

   * - **Name in GUROBI**
     - **Option name in AIMMS**
   * - AGGFILL
     - :ref:`GUROBI_Presolve_-_Presolve_Aggregation_Fill`
   * - AGGREGATE
     - :ref:`GUROBI_Presolve_-_Presolve_Aggregation`
   * - BARCONVTOL
     - :ref:`GUROBI_Barrier_-_Barrier_Convergence_Tolerance`
   * - BARCORRECTORS
     - :ref:`GUROBI_Barrier_-_Barrier_Correction_Steps`
   * - BARHOMOGENEOUS
     - :ref:`GUROBI_Barrier_-_Barrier_Homogeneous_Aalgorithm`
   * - BARITERLIMIT
     - :ref:`GUROBI_Barrier_-_Barrier_Iteration_Limit`
   * - BARORDER
     - :ref:`GUROBI_Barrier_-_Barrier_Ordering`
   * - BARQCPCONVTOL
     - :ref:`GUROBI_Barrier_-_Barrier_QCP_Convergence_Tol`
   * - BESTBDSTOP
     - :ref:`GUROBI_MIP_-_MIP_Best_Bound_Stop`
   * - BESTOBJSTOP
     - :ref:`GUROBI_MIP_-_MIP_Best_Objective_Stop`
   * - BQPCUTS
     - :ref:`GUROBI_MIP_Cuts_-_BQP_Cuts`
   * - BRANCHDIR
     - :ref:`GUROBI_MIP_-_Branch_direction`
   * - CLIQUECUTS
     - :ref:`GUROBI_MIP_Cuts_-_Clique_Cuts`
   * - CONCURRENTMETHOD
     - :ref:`GUROBI_General_-_Concurrent_Method`
   * - CONCURRENTMIP
     - :ref:`GUROBI_Parallel_-_Concurrent_MIP`
   * - COVERCUTS
     - :ref:`GUROBI_MIP_Cuts_-_Cover_Cuts`
   * - CROSSOVER
     - :ref:`GUROBI_Barrier_-_Barrier_Crossover`
   * - CROSSOVERBASIS
     - :ref:`GUROBI_Barrier_-_Barrier_Crossover_Basis`
   * - CUTAGGPASSES
     - :ref:`GUROBI_MIP_Cuts_-_Cut_Aggr_Passes_Limit`
   * - CUTPASSES
     - :ref:`GUROBI_MIP_Cuts_-_Root_Cut_Passes_Limit`
   * - CUTS
     - :ref:`GUROBI_MIP_Cuts_-_Global_Cut_Control`
   * - DEGENMOVES
     - :ref:`GUROBI_Simplex_-_Degenerate_Simplex_Moves_Limit`
   * - DISCONNECTED
     - :ref:`GUROBI_MIP_-_Disconnected_Component_Strateg`
   * - DISPLAYINTERVAL
     - :ref:`GUROBI_Logging_-_Output_File_Display_Interval`
   * - DUALIMPLIEDCUTS
     - :ref:`GUROBI_MIP_Cuts_-_Dual_Implied_Cuts`
   * - DUALREDUCTIONS
     - :ref:`GUROBI_Presolve_-_Dual_Reductions`
   * - FEASIBILITYTOL
     - :ref:`GUROBI_General_-_Feasibility`
   * - FEASRELAXBIGM
     - :ref:`GUROBI_General_-_FeasRelax_big-M`
   * - FLOWCOVERCUTS
     - :ref:`GUROBI_MIP_Cuts_-_Flow_Cover_Cuts`
   * - FLOWPATHCUTS
     - :ref:`GUROBI_MIP_Cuts_-_Flow_Path_Cuts`
   * - GOMORYPASSES
     - :ref:`GUROBI_MIP_Cuts_-_Gomory_Cuts_Passes_L`
   * - GUBCOVERCUTS
     - :ref:`GUROBI_MIP_Cuts_-_GUB_Cover_Cuts`
   * - HEURISTICS
     - :ref:`GUROBI_MIP_Heuristic_-_Heuristics`
   * - IISMETHOD
     - :ref:`GUROBI_General_-_IIS_Method`
   * - IMPLIEDCUTS
     - :ref:`GUROBI_MIP_Cuts_-_Implied_Bound_Cuts`
   * - IMPROVESTARTGAP
     - :ref:`GUROBI_MIP_-_Improve_Start_Gap`
   * - IMPROVESTARTNODES
     - :ref:`GUROBI_MIP_-_Improve_Start_Nodes`
   * - IMPROVESTARTTIME
     - :ref:`GUROBI_MIP_-_Improve_Start_Time`
   * - INFPROOFCUTS
     - :ref:`GUROBI_MIP_Cuts_-_Infeasibility_Proof_Cuts`
   * - INTEGRALITYFOCUS
     - :ref:`GUROBI_MIP_-_Integrality_Focus`
   * - INTFEASTOL
     - :ref:`GUROBI_MIP_-_Integrality`
   * - LIFTPROJECTCUTS
     - :ref:`GUROBI_MIP_Cuts_-_Lift_and_Project_Cuts`
   * - LOGTOCONSOLE
     - :ref:`GUROBI_Logging_-_Log_to_Console`
   * - LPWARMSTART
     - :ref:`GUROBI_General_-_Warm_Start`
   * - MARKOWITZTOL
     - :ref:`GUROBI_Simplex_-_Markowitz`
   * - MEMLIMIT
     - :ref:`GUROBI_General_-_Memory_Limit`
   * - METHOD
     - :ref:`GUROBI_General_-_Method`
   * - MINRELNODES
     - :ref:`GUROBI_MIP_Heuristic_-_Minimum_Relaxation_Heuristic_N`
   * - MIPFOCUS
     - :ref:`GUROBI_MIP_-_MIP_Focus`
   * - MIPSEPCUTS
     - :ref:`GUROBI_MIP_Cuts_-_MIP_Separation_Cuts`
   * - MIQCPMETHOD
     - :ref:`GUROBI_Quadratic_-_MIQCP_Method`
   * - MIRCUTS
     - :ref:`GUROBI_MIP_Cuts_-_MIR_Cuts`
   * - MIXINGCUTS
     - :ref:`GUROBI_MIP_Cuts_-_Mixing_Cuts`
   * - MODKCUTS
     - :ref:`GUROBI_MIP_Cuts_-_Mod_K_cuts`
   * - MULTIOBJMETHOD
     - :ref:`GUROBI_General_-_Multi_objective_method`
   * - MULTIOBJPRE
     - :ref:`GUROBI_Presolve_-_Multi_Objective_Presolve`
   * - NETWORKALG
     - :ref:`GUROBI_Simplex_-_Network_Algorithm`
   * - NETWORKCUTS
     - :ref:`GUROBI_MIP_Cuts_-_Network_Cuts`
   * - NLPHEUR
     - :ref:`GUROBI_Quadratic_-_NLP_Heuristic`
   * - NODEFILESTART
     - :ref:`GUROBI_MIP_-_Node_File_Start`
   * - NODELIMIT
     - :ref:`GUROBI_MIP_-_Node_Limit`
   * - NODEMETHOD
     - :ref:`GUROBI_MIP_-_MIP_Node_Method`
   * - NONCONVEX
     - :ref:`GUROBI_Quadratic_-_Nonconvex_Strategy`
   * - NORELHEURTIME
     - :ref:`GUROBI_MIP_Heuristic_-_No_Relaxation_Heuristic_Time`
   * - NORELHEURWORK
     - :ref:`GUROBI_MIP_Heuristic_-_No_Relaxation_Heuristic_Work`
   * - NORMADJUST
     - :ref:`GUROBI_Simplex_-_Norm_Adjust`
   * - NUMERICFOCUS
     - :ref:`GUROBI_General_-_Numeric_Focus`
   * - OBBT
     - :ref:`GUROBI_MIP_Presolve_-_MIP_OBBT`
   * - OBJSCALE
     - :ref:`GUROBI_Simplex_-_Objective_Scale`
   * - OPTIMALITYTOL
     - :ref:`GUROBI_General_-_Optimality`
   * - OUTPUTFLAG
     - :ref:`GUROBI_Logging_-_Output_File`
   * - PARTITIONPLACE
     - :ref:`GUROBI_MIP_Heuristic_-_Partition_Heuristic`
   * - PERTURBVALUE
     - :ref:`GUROBI_Simplex_-_Perturbation`
   * - POOLGAP
     - :ref:`GUROBI_Solution_Pool_-_Pool_Gap`
   * - POOLGAPABS
     - :ref:`GUROBI_Solution_Pool_-_Pool_Absolute_Gap`
   * - POOLSEARCHMODE
     - :ref:`GUROBI_Solution_Pool_-_Pool_Search_Mode`
   * - POOLSOLUTIONS
     - :ref:`GUROBI_Solution_Pool_-_Pool_Size`
   * - PREDEPROW
     - :ref:`GUROBI_Presolve_-_Presolve_Row_Reduction`
   * - PREDUAL
     - :ref:`GUROBI_Presolve_-_Presolve_Dual`
   * - PREMIQCPFORM
     - :ref:`GUROBI_Quadratic_-_MIQCP_Formulation`
   * - PREPASSES
     - :ref:`GUROBI_Presolve_-_Presolve_Passes`
   * - PREQLINEARIZE
     - :ref:`GUROBI_Presolve_-_Linearize_Quadratic_Constraint`
   * - PRESOLVE
     - :ref:`GUROBI_Presolve_-_Presolve`
   * - PRESOS1BIGM
     - :ref:`GUROBI_MIP_Presolve_-_SOS1_Reformulation_Threshold`
   * - PRESOS1ENCODING
     - :ref:`GUROBI_MIP_Presolve_-_SOS1_Encoding`
   * - PRESOS2BIGM
     - :ref:`GUROBI_MIP_Presolve_-_SOS2_Reformulation_Threshold`
   * - PRESOS2ENCODING
     - :ref:`GUROBI_MIP_Presolve_-_SOS2_Encoding`
   * - PRESPARSIFY
     - :ref:`GUROBI_MIP_Presolve_-_Presolve_Sparsify_Reduction`
   * - PROJIMPLIEDCUTS
     - :ref:`GUROBI_MIP_Cuts_-_Projected_Implied_Bound_Cuts`
   * - PSDTOL
     - :ref:`GUROBI_Quadratic_-_PSD_Tolerance`
   * - PUMPPASSES
     - :ref:`GUROBI_MIP_Heuristic_-_Feasibility_Pump_Passes`
   * - QCPDUAL
     - :ref:`GUROBI_Quadratic_-_QCP_Dual_Values`
   * - QUAD
     - :ref:`GUROBI_Simplex_-_Quad_Precision`
   * - RELAXLIFTCUTS
     - :ref:`GUROBI_MIP_Cuts_-_Relax-and-lift_Cuts`
   * - RINS
     - :ref:`GUROBI_MIP_Heuristic_-_RINS_Heuristic_Frequency`
   * - RLTCUTS
     - :ref:`GUROBI_MIP_Cuts_-_RLT_Cuts`
   * - SCALEFLAG
     - :ref:`GUROBI_General_-_Scale`
   * - SEED
     - :ref:`GUROBI_General_-_Random_Seed`
   * - SIFTING
     - :ref:`GUROBI_Simplex_-_Sifting`
   * - SIFTMETHOD
     - :ref:`GUROBI_Simplex_-_Sifting_Method`
   * - SIMPLEXPRICING
     - :ref:`GUROBI_Simplex_-_Pricing`
   * - SOFTMEMLIMIT
     - :ref:`GUROBI_General_-_Soft_Memory_Limit`
   * - SOLUTIONTARGET
     - :ref:`GUROBI_General_-_Solution_Target`
   * - STARTNODELIMIT
     - :ref:`GUROBI_MIP_-_MIP_Start_Node_Limit`
   * - STRONGCGCUTS
     - :ref:`GUROBI_MIP_Cuts_-_Strong_CG_Cuts`
   * - SUBMIPCUTS
     - :ref:`GUROBI_MIP_Cuts_-_Sub_MIP_Cuts`
   * - SUBMIPNODES
     - :ref:`GUROBI_MIP_Heuristic_-_RINS_Sub_Node_Lim`
   * - SYMMETRY
     - :ref:`GUROBI_MIP_-_MIP_Symmetry`
   * - THREADS
     - :ref:`GUROBI_Parallel_-_Thread_Limit`
   * - TUNECLEANUP
     - :ref:`GUROBI_Tuning_-_Tune_Cleanup`
   * - TUNECRITERION
     - :ref:`GUROBI_Tuning_-_Tune_Criterion`
   * - TUNEMETRIC
     - :ref:`GUROBI_Tuning_-_Tune_Metric`
   * - TUNEOUTPUT
     - :ref:`GUROBI_Logging_-_Tune_Output_Level`
   * - TUNERESULTS
     - :ref:`GUROBI_Tuning_-_Tune_Results`
   * - TUNETARGETMIPGAP
     - :ref:`GUROBI_Tuning_-_Tune_Target_MIP_Gap`
   * - TUNETARGETTIME
     - :ref:`GUROBI_Tuning_-_Tune_Target_Time`
   * - TUNETIMELIMIT
     - :ref:`GUROBI_Tuning_-_Tune_Time_Limit`
   * - TUNETRIALS
     - :ref:`GUROBI_Tuning_-_Tune_Trials`
   * - VARBRANCH
     - :ref:`GUROBI_MIP_-_Select_Variables`
   * - WORKLIMIT
     - :ref:`GUROBI_General_-_Work_Limit`
   * - ZEROHALFCUTS
     - :ref:`GUROBI_MIP_Cuts_-_Zero_Half_Cuts`
   * - ZEROOBJNODES
     - :ref:`GUROBI_MIP_Heuristic_-_Zero_Objective_Node_Limit`


**Note** 

*	The Gurobi parameter PRECRUSH is not available in AIMMS. AIMMS automatically switches it on when a cut callback procedure is installed in the AIMMS model.
