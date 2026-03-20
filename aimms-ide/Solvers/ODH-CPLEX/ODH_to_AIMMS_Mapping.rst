

.. _ODH_to_AIMMS_Mapping:


ODH to AIMMS Mapping
========================

**ODH engine parameters** 

The table below shows in the left column the ODH engine parameters from ODH-CPLEX that can be set in AIMMS; the right column displays for each ODH-CPLEX 5.3 parameter the associated AIMMS option.

.. list-table::

   * - **Name in ODH-CPLEX**
     - **Option name in AIMMS**
   * - DECOMPDENSITY
     - :doc:`Advanced - Decomposition Density <Advanced/ODH_Advanced_-_Decomposition_Density>`
   * - DETERMINISTIC
     - :doc:`Heuristics - Solution Improvement Heuristic Mode <Heuristics/ODH_Heuristic_-_Sol_Impr_Heur_Mode>`
   * - DIVISOR
     - :doc:`Advanced - Initial Divisor Value Sub Models <Advanced/ODH_Advanced_-_Initial_Divisor_Value_Sub>`
   * - FEASOPT
     - :doc:`Advanced - Optimization Method <Advanced/ODH_Advanced_-_Optimization_Method>`
   * - FEASTOL
     - :doc:`General - ODH Feasibility Tolerance <General/ODH_General_-_ODH_Feasibility_Tolerance>`
   * - FIRSTFEAS
     - :doc:`Heuristics - First Feasible Heuristic <Heuristics/ODH_Heuristic_-_First_Feasible_Heuristic>`
   * - FIRSTFEASCONTINUE
     - :doc:`Heuristics - First Feasible Heuristic Continue <Heuristics/ODH_Heuristic_-_First_Feasible_Heuristic_Continue>`
   * - FIRSTFEASEFFORT
     - :doc:`Heuristics - First Feasible Heuristic Effort Level <Heuristics/ODH_Heuristic_-_First_Feasible_Heuristic_Effort_Level>`
   * - FIRSTFEASSHIFT
     - :doc:`Heuristics - First Feasible Heuristic Shift <Heuristics/ODH_Heuristic_-_First_Feasible_Heuristic_Shift>`
   * - GLOBALBOUNDS
     - :doc:`Advanced - Global Bounds <Advanced/ODH_Advanced_-_Global_Bounds>`
   * - INTERDIV
     - :doc:`Advanced - Initial Divisor Value <Advanced/ODH_Advanced_-_Initial_Divisor_Value>`
   * - MAXBACKTRACK
     - :doc:`Advanced - Backtrack Limit <Advanced/ODH_Advanced_-_Backtrack_Limit>`
   * - MAXINFREPEAT
     - :doc:`Advanced - Maximum Divisor Repeats Infeasible <Advanced/ODH_Advanced_-_Maximum_Divisor_Repeats_Inf>`
   * - MAXINTERDIV
     - :doc:`Advanced - Maximum Divisor Value <Advanced/ODH_Advanced_-_Maximum_Divisor_Value>`
   * - MAXREPEAT
     - :doc:`Advanced - Maximum Divisor Repeats <Advanced/ODH_Advanced_-_Maximum_Divisor_Repeats>`
   * - OBJTARGET
     - :doc:`General - Objective Target <General/ODH_General_-_Objective_Target>`
   * - ODHPRESOLVE
     - :doc:`General - ODH Presolve <General/ODH_General_-_ODH_Presolve>`
   * - PENALTY
     - :doc:`Heuristics - Solution Improvement Heuristic Penalty <Heuristics/ODH_Heuristic_-_Sol_Impr_Heur_Penalty>`
   * - PHASE12
     - :doc:`General - Remove Infeasibilities Method <General/ODH_General_-_Remove_Inf_Method>`
   * - PRESOLVE
     - :doc:`General - Presolve <General/ODH_General_-_Presolve>`
   * - PROCESSORLOCK
     - :doc:`Parallel - Processor Lock <Parallel/ODH_Parallel_-_Processor_Lock>`
   * - QUICKFIRSTSOLVE
     - :doc:`General - Quick First Solve <General/ODH_General_-_Quick_First_Solve>`
   * - RECURSE
     - :doc:`Heuristics - Recurse <Heuristics/ODH_Heuristic_-_Recurse>`
   * - RECURSEDECOMP
     - :doc:`Heuristics - Recurse Decomposition Method <Heuristics/ODH_Heuristic_-_Recurse_Decomposition_Method>`
   * - RECURSEITERLIM
     - :doc:`Heuristics - Recurse Iteration Limit <Heuristics/ODH_Heuristic_-_Recurse_Iteration_Limit>`
   * - RECURSELOG
     - :doc:`Logging - Recurse Log <Logging/ODH_Logging_-_Recurse_Log>`
   * - RECURSEMINITERLIM
     - :doc:`Heuristics - Recurse Minimum Iterations <Heuristics/ODH_Heuristic_-_Recurse_Minimum_Iterations>`
   * - RECURSESOLITERLIM
     - :doc:`Heuristics - Recurse Iteration Limit Solution <Heuristics/ODH_Heuristic_-_Recurse_Iteration_Limit_Solution>`
   * - REJECTINFSOL
     - :doc:`General - Reject Infeasible Solutions <General/ODH_General_-_Reject_Inf_Solutions>`
   * - RELAXSOS2
     - :doc:`General - Relax SOS2 <General/ODH_General_-_Relax_SOS2>`
   * - SEED
     - :doc:`General - ODH Seed <General/ODH_General_-_ODH_Seed>`
   * - STRATEGY
     - :doc:`Heuristics - Solution Improvement Heuristic Strategy <Heuristics/ODH_Heuristic_-_Sol_Impr_Heur_Strategy>`
   * - SYNCFREQ
     - :doc:`Parallel - Thread Synchronization Frequency <Parallel/ODH_Parallel_-_Thread_Sync_Freq>`
   * - THREADLOG
     - :doc:`Logging - Thread Log <Logging/ODH_Logging_-_Thread_Log>`
   * - THREADS
     - :doc:`Parallel - Thread Limit <Parallel/ODH_Parallel_-_Thread_Limit>`
   * - TIMELIMIT
     - :doc:`Stop Criteria - Time Limit <../../Aimms/Options/Solvers General/Stop Criteria/Stop_Criteria_-_Time_Limit>`
   * - VARIABLECLEAN
     - :doc:`General - Clean Variables Sub Models <General/ODH_General_-_Clean_variables_sub_models>`
   * - WRITESOLUTION
     - :doc:`General - Write Solution File <General/ODH_General_-_Write_Solution_File>`


**Main CPLEX solve parameters** 

The table below shows CPLEX options for the main CPLEX solve in ODH-CPLEX (if the **Search Mode**  is set to 'Global Solution') or for getting an initial feasible solution (if the **Search Mode**  is set to 'Local Solution'). 
The table below shows in the left column the CPLEX parameters from ODH-CPLEX that can be set in AIMMS; the right column displays for each ODH-CPLEX 5.3 parameter the associated AIMMS option.

.. list-table::

   * - **Name in ODH-CPLEX**
     - **Option name in AIMMS**
   * - CPX_ADVIND
     - :doc:`CPLEX General - Advanced Start <CPLEX General/ODH_XGeneral_-_AdvancedStart>`
   * - CPX_AGGCUTLIM
     - :doc:`CPLEX MIP Cuts - Cut Generation Limit <CPLEX MIP Cuts/ODH_XCuts_-_Cut_Gen_Limi>`
   * - CPX_AGGFILL
     - :doc:`CPLEX Preprocessing - Limit Substitutions <CPLEX Preprocessing/ODH_XPrepr_-_Limit_Substitut>`
   * - CPX_AGGIND
     - :doc:`CPLEX Preprocessing - Aggregator <CPLEX Preprocessing/ODH_XPrepr_-_Aggregator>`
   * - CPX_AUXROOTTHREADS
     - :doc:`CPLEX Parallel - Auxiliary Root Threads <CPLEX Parallel/ODH_XPar_-_Auxiliary_Root_Threads>`
   * - CPX_BARALG
     - :doc:`CPLEX Barrier - Barrier Algorithm <CPLEX Barrier/ODH_XBarrier_-_Barrier_Algorithm>`
   * - CPX_BARCOLNZ
     - :doc:`CPLEX Barrier - Barrier Density Definition <CPLEX Barrier/ODH_XBarrier_-_Barrier_Density_Defi>`
   * - CPX_BARCROSSALG
     - :doc:`CPLEX Barrier - Barrier Crossover Algorithm <CPLEX Barrier/ODH_XBarrier_-_Barrier_cross>`
   * - CPX_BARDISPLAY
     - :doc:`CPLEX Logging - Barrier Display <CPLEX Logging/ODH_XLogging_-_Barrier_Display>`
   * - CPX_BAREPCOMP
     - :doc:`CPLEX Barrier - Barrier Convergence Tolerance <CPLEX Barrier/ODH_XBarrier_-_Barrier_Convergence_>`
   * - CPX_BARGROWTH
     - :doc:`CPLEX Barrier - Barrier Growth Limit <CPLEX Barrier/ODH_XBarrier_-_Barrier_Growth_Limit>`
   * - CPX_BARITLIM
     - :doc:`CPLEX Barrier - Barrier Iterations <CPLEX Barrier/ODH_XBarrier_-_Barrier_Iterations>`
   * - CPX_BARMAXCOR
     - :doc:`CPLEX Barrier - Barrier Maximal Number of Corrections <CPLEX Barrier/ODH_XBarrier_-_Barrier_Maximal_Numb>`
   * - CPX_BAROBJRNG
     - :doc:`CPLEX Barrier - Barrier Objective Range <CPLEX Barrier/ODH_XBarrier_-_Barrier_Objective_Ra>`
   * - CPX_BARORDER
     - :doc:`CPLEX Barrier - Barrier Ordering <CPLEX Barrier/ODH_XBarrier_-_Barrier_Ordering>`
   * - CPX_BARQCPEPCOMP
     - :doc:`CPLEX Quadratic - Barrier Convergence Tolerance for QCP <CPLEX Quadratic/ODH_XQuadratic_-_Barrier_Conv_Toler>`
   * - CPX_BARSTARTALG
     - :doc:`CPLEX Barrier - Barrier Start Algorithm <CPLEX Barrier/ODH_XBarrier_-_Barrier_Start_Algori>`
   * - CPX_BNDSTRENIND
     - :doc:`CPLEX MIP Preprocessing - Boundstrength <CPLEX MIP Preprocessing/ODH_XMIP_Prepr_-_Boundstreng>`
   * - CPX_BQPCUTS
     - :doc:`CPLEX MIP Cuts - BQP Cuts <CPLEX MIP Cuts/ODH_XCuts_-_BQP_Cuts>`
   * - CPX_BRDIR
     - :doc:`CPLEX MIP - Branch <CPLEX MIP/ODH_XMIP_-_Branch>`
   * - CPX_BTTOL
     - :doc:`CPLEX MIP - Backtrack <CPLEX MIP/ODH_XMIP_-_Backtrack>`
   * - CPX_CLIQUES
     - :doc:`CPLEX MIP Cuts - Clique Cuts <CPLEX MIP Cuts/ODH_XCuts_-_Clique_Cuts>`
   * - CPX_CLOCKTYPE
     - :doc:`CPLEX General - Clock Type <CPLEX General/ODH_XGeneral_-_Clock_Type>`
   * - CPX_CLONELOG
     - :doc:`CPLEX Logging - Clone Log Files <CPLEX Logging/ODH_XLogging_-_Clone_Log_Files>`
   * - CPX_COEREDIND
     - :doc:`CPLEX MIP Preprocessing - Coefficient Reduction <CPLEX MIP Preprocessing/ODH_XMIP_Prepr_-_Coef_Reduc>`
   * - CPX_CONFLICTALG
     - :doc:`CPLEX General - Conflict Algorithm <CPLEX General/ODH_XGeneral_-_Conflict_Algorithm>`
   * - CPX_COVERS
     - :doc:`CPLEX MIP Cuts - Cover Cuts <CPLEX MIP Cuts/ODH_XCuts_-_Cover_Cuts>`
   * - CPX_CRAIND
     - :doc:`CPLEX Simplex - Crash Ordering <CPLEX Simplex/ODH_XSimplex_-_Crash_Ordering>`
   * - CPX_CUTLO
     - :doc:`MIP Options - Cutoff <../../Aimms/Options/Solvers General/MIP Options/MIP_Options_-_Cutoff>`
   * - CPX_CUTPASS
     - :doc:`CPLEX MIP Cuts - MIP Number of Cut Passes <CPLEX MIP Cuts/ODH_XCuts_-_MIP_Nr_of_Cut_Pa>`
   * - CPX_CUTSFACTOR
     - :doc:`CPLEX MIP Cuts - Cuts Factor <CPLEX MIP Cuts/ODH_XCuts_-_Cuts_Factor>`
   * - CPX_CUTUP
     - :doc:`MIP Options - Cutoff <../../Aimms/Options/Solvers General/MIP Options/MIP_Options_-_Cutoff>`
   * - CPX_DATACHECK
     - :doc:`CPLEX General - Data Check and Modeling Assistance <CPLEX General/ODH_XGeneral_-_Data_Check>`
   * - CPX_DEPIND
     - :doc:`CPLEX Preprocessing - Dependency <CPLEX Preprocessing/ODH_XPrepr_-_Dependency>`
   * - CPX_DETTILIM
     - :doc:`CPLEX General - Deterministic Time Limit <CPLEX General/ODH_XGeneral_-_Deterministic_Time_Limit>`
   * - CPX_DISJCUTS
     - :doc:`CPLEX MIP Cuts - Disjunctive Cuts <CPLEX MIP Cuts/ODH_XCuts_-_Disjunct_Cuts>`
   * - CPX_DIVETYPE
     - :doc:`CPLEX MIP - MIP Dive Strategy <CPLEX MIP/ODH_XMIP_-_MIP_Dive_Strat>`
   * - CPX_DPRIIND
     - :doc:`CPLEX Simplex - Dual Pricing Algorithm <CPLEX Simplex/ODH_XSimplex_-_Dual_Pric_Alg>`
   * - CPX_DYNAMICROWS
     - :doc:`CPLEX Simplex - Dynamic Row Management <CPLEX Simplex/ODH_XSimplex_-_Dynamic_Row_Management>`
   * - CPX_EACHCUTLIM
     - :doc:`CPLEX MIP Cuts - Cut Limit <CPLEX MIP Cuts/ODH_XCuts_-_Cut_Limit>`
   * - CPX_EPAGAP
     - :doc:`MIP Options - MIP Absolute Optimality Tolerance <../../Aimms/Options/Solvers General/MIP Options/MIP_Options_-_MIP_Absolute_Opt>`
   * - CPX_EPGAP
     - :doc:`MIP Options - MIP Relative Optimality Tolerance <../../Aimms/Options/Solvers General/MIP Options/MIP_Options_-_MIP_Relative_Opt>`
   * - CPX_EPINT
     - :doc:`CPLEX MIP - Integrality <CPLEX MIP/ODH_XMIP_-_Integrality>`
   * - CPX_EPMRK
     - :doc:`CPLEX Simplex - Markowitz <CPLEX Simplex/ODH_XSimplex_-_Markowitz>`
   * - CPX_EPOPT
     - :doc:`CPLEX Simplex - Optimality <CPLEX Simplex/ODH_XSimplex_-_Optimality>`
   * - CPX_EPPER
     - :doc:`CPLEX Simplex - Perturbation Constant <CPLEX Simplex/ODH_XSimplex_-_Perturb_Const>`
   * - CPX_EPRHS
     - :doc:`CPLEX Simplex - Feasibility <CPLEX Simplex/ODH_XSimplex_-_Feasibility>`
   * - CPX_FLOWCOVERS
     - :doc:`CPLEX MIP Cuts - Flow Cover Cuts <CPLEX MIP Cuts/ODH_XCuts_-_Flow_Cover_Cuts>`
   * - CPX_FLOWPATHS
     - :doc:`CPLEX MIP Cuts - Flow Path Cuts <CPLEX MIP Cuts/ODH_XCuts_-_Flow_Path_Cuts>`
   * - CPX_FOLDING
     - :doc:`CPLEX Preprocessing - Folding <CPLEX Preprocessing/ODH_XPrepr_-_Folding>`
   * - CPX_FPHEUR
     - :doc:`CPLEX MIP Heuristics - Feasibility Pump Heuristic <CPLEX MIP Heuristics/ODH_XMIP_Heuristic_-_Feasibility_Pump_Heuristic>`
   * - CPX_FRACCAND
     - :doc:`CPLEX MIP Cuts - Gomory Cuts Candidate Limit <CPLEX MIP Cuts/ODH_XCuts_-_Gomory_Cuts_Cand>`
   * - CPX_FRACCUTS
     - :doc:`CPLEX MIP Cuts - Gomory Cuts <CPLEX MIP Cuts/ODH_XCuts_-_Gomory_Cuts>`
   * - CPX_FRACPASS
     - :doc:`CPLEX MIP Cuts - Gomory Cuts Pass Limit <CPLEX MIP Cuts/ODH_XCuts_-_Gomory_Cuts_Pass_L>`
   * - CPX_GUBCOVERS
     - :doc:`CPLEX MIP Cuts - GUB Cover Cuts <CPLEX MIP Cuts/ODH_XCuts_-_GUB_Cover_Cuts>`
   * - CPX_HEUREFFORT
     - :doc:`CPLEX MIP Heuristics - Heuristic Effort <CPLEX MIP Heuristics/ODH_XMIP_Heuristic_-_Heuristic_Effort>`
   * - CPX_HEURFREQ
     - :doc:`CPLEX MIP Heuristics - Heuristic Frequency <CPLEX MIP Heuristics/ODH_XMIP_Heuristic_-_Heuristic_Freq>`
   * - CPX_IMPLBD
     - :doc:`CPLEX MIP Cuts - Implied Bound Cuts <CPLEX MIP Cuts/ODH_XCuts_-_Implied_Bound_Cuts>`
   * - CPX_INTSOLLIM
     - :doc:`MIP Options - Maximal Number of Integer Solutions <../../Aimms/Options/Solvers General/MIP Options/MIP_Options_-_Maximal_Number_o>`
   * - CPX_ITLIM
     - :doc:`Stop Criteria - Iteration Limit <../../Aimms/Options/Solvers General/Stop Criteria/Stop_Criteria_-_Iteration_Limi>`
   * - CPX_LANDPCUTS
     - :doc:`CPLEX MIP Cuts - Lift and Project Cuts <CPLEX MIP Cuts/ODH_XCuts_-_Lift_and_Project_Cuts>`
   * - CPX_LBHEUR
     - :doc:`CPLEX MIP Heuristics - Local Branching Heuristic <CPLEX MIP Heuristics/ODH_XMIP_Heuristic_-_Local_Branch_Heur>`
   * - CPX_LOCALIMPLBD
     - :doc:`CPLEX MIP Cuts - Local Implied Bound Cuts <CPLEX MIP Cuts/ODH_XCuts_-_Local_Implied_Bound_Cuts>`
   * - CPX_MCFCUTS
     - :doc:`CPLEX MIP Cuts - MCF Cuts <CPLEX MIP Cuts/ODH_XCuts_-_MCF_Cuts>`
   * - CPX_MEMORYEMPHASIS
     - :doc:`CPLEX General - Memory Emphasis <CPLEX General/ODH_XGeneral_-_MemoryEmphasis>`
   * - CPX_MIPDISPLAY
     - :doc:`CPLEX Logging - MIP Display <CPLEX Logging/ODH_XLogging_-_MIP_Display>`
   * - CPX_MIPEMPHASIS
     - :doc:`CPLEX MIP - MIP Emphasis <CPLEX MIP/ODH_XMIP_-_MIP_Emphasis>`
   * - CPX_MIPINTERVAL
     - :doc:`CPLEX Logging - MIP Interval <CPLEX Logging/ODH_XLogging_-_MIP_Interval>`
   * - CPX_MIPORDIND
     - :doc:`CPLEX MIP - MIP Priority Order Switch <CPLEX MIP/ODH_XMIP_-_MIP_Priority_Order_Switch>`
   * - CPX_MIPORDTYPE
     - :doc:`CPLEX MIP - MIP Priority Order Type <CPLEX MIP/ODH_XMIP_-_MIP_Priority_Order_Type>`
   * - CPX_MIPSEARCH
     - :doc:`CPLEX MIP - MIP Search Strategy <CPLEX MIP/ODH_XMIP_-_MIP_Search_Strategy>`
   * - CPX_MIQCPSTRAT
     - :doc:`CPLEX Quadratic - MIQCP Strategy <CPLEX Quadratic/ODH_XQuadratic_-_MIQCP_Strategy>`
   * - CPX_MIRCUTS
     - :doc:`CPLEX MIP Cuts - Mixed Integer Rounding Cuts <CPLEX MIP Cuts/ODH_XCuts_-_Mix_Integer_Round>`
   * - CPX_NETEPOPT
     - :doc:`CPLEX Network - Network Optimality <CPLEX Network/ODH_XNetwork_-_Network_Optimality>`
   * - CPX_NETEPRHS
     - :doc:`CPLEX Network - Network Feasibility <CPLEX Network/ODH_XNetwork_-_Network_Feasibility>`
   * - CPX_NETITLIM
     - :doc:`CPLEX Network - Network Iterations <CPLEX Network/ODH_XNetwork_-_Network_Iterations>`
   * - CPX_NETPPRIIND
     - :doc:`CPLEX Network - Network Pricing <CPLEX Network/ODH_XNetwork_-_Network_Pricing>`
   * - CPX_NODECUTS
     - :doc:`CPLEX MIP Cuts - Node Cuts <CPLEX MIP Cuts/ODH_XCuts_-_Node_Cuts>`
   * - CPX_NODEFILEIND
     - :doc:`CPLEX MIP - Node File <CPLEX MIP/ODH_XMIP_-_Node_File>`
   * - CPX_NODELIM
     - :doc:`CPLEX MIP - Maximal Number of Nodes <CPLEX MIP/ODH_XMIP_-_Max_Nr_of_Nodes>`
   * - CPX_NODESEL
     - :doc:`CPLEX MIP - Selection of Nodes <CPLEX MIP/ODH_XMIP_-_Selection_of_Nodes>`
   * - CPX_NUMERICALEMPHASIS
     - :doc:`CPLEX General - Numerical Emphasis <CPLEX General/ODH_XGeneral_-_NumericalEmphasis>`
   * - CPX_OBJDIF
     - :doc:`CPLEX MIP - Difference Objective <CPLEX MIP/ODH_XMIP_-_Difference_Object>`
   * - CPX_OPTIMALITYTARGET
     - :doc:`CPLEX Quadratic - Solution Target <CPLEX Quadratic/ODH_XQuadratic_-_Solution_Target>`
   * - CPX_PARALLELMODE
     - :doc:`CPLEX Parallel - Parallel Mode <CPLEX Parallel/ODH_XPar_-_Parallel_Mode>`
   * - CPX_PERIND
     - :doc:`CPLEX Simplex - Perturbation Indicator <CPLEX Simplex/ODH_XSimplex_-_Perturb_Indic>`
   * - CPX_PERLIM
     - :doc:`CPLEX Simplex - Stalled Iterations <CPLEX Simplex/ODH_XSimplex_-_Stalled_Iter>`
   * - CPX_POLISHAFTERDETTIME
     - :doc:`CPLEX MIP Solution Polishing - Polishing Time Deterministic <CPLEX MIP Solution Polishing/ODH_XPolishing_Time_Deterministic>`
   * - CPX_POLISHAFTEREPAGAP
     - :doc:`CPLEX MIP Solution Polishing - Polishing Absolute MIP Gap <CPLEX MIP Solution Polishing/ODH_XPolishing_Absolute_MIP_Gap>`
   * - CPX_POLISHAFTEREPGAP
     - :doc:`CPLEX MIP Solution Polishing - Polishing Relative MIP Gap <CPLEX MIP Solution Polishing/ODH_XPolishing_Relative_MIP_Gap>`
   * - CPX_POLISHAFTERINTSOL
     - :doc:`CPLEX MIP Solution Polishing - Polishing Number of Solutions <CPLEX MIP Solution Polishing/ODH_XPolishing_Number_of_Solutions>`
   * - CPX_POLISHAFTERNODE
     - :doc:`CPLEX MIP Solution Polishing - Polishing Number of Nodes <CPLEX MIP Solution Polishing/ODH_XPolishing_Number_of_Nodes>`
   * - CPX_POLISHAFTERTIME
     - :doc:`CPLEX MIP Solution Polishing - Polishing Time <CPLEX MIP Solution Polishing/ODH_XPolishing_Time>`
   * - CPX_POPULATELIM
     - :doc:`CPLEX MIP Solution Pool - Population Limit <CPLEX MIP Solution Pool/ODH_XMIP_Solp_-_Population_Limit>`
   * - CPX_PREDUAL
     - :doc:`CPLEX Preprocessing - Presolve Pass Dual <CPLEX Preprocessing/ODH_XPrepr_-_Presolve_Pass_D>`
   * - CPX_PREPASS
     - :doc:`CPLEX Preprocessing - Number of Iterations in Presolve <CPLEX Preprocessing/ODH_XPrepr_-_Number_of_IterP>`
   * - CPX_PRESLVND
     - :doc:`CPLEX MIP - MIP Node Presolve <CPLEX MIP/ODH_XMIP_-_MIP_Node_Presolve>`
   * - CPX_PRICELIM
     - :doc:`CPLEX Simplex - Pricing <CPLEX Simplex/ODH_XSimplex_-_Pricing>`
   * - CPX_PROBE
     - :doc:`CPLEX MIP - MIP Probing <CPLEX MIP/ODH_XMIP_-_MIP_Probing>`
   * - CPX_PROBEDETTIME
     - :doc:`CPLEX MIP - Probing Time Deterministic <CPLEX MIP/ODH_XMIP_-_Probing_Time_Deterministic>`
   * - CPX_PROBETIME
     - :doc:`CPLEX MIP - Probing Time <CPLEX MIP/ODH_XMIP_-_Probing_Time>`
   * - CPX_PPRIIND
     - :doc:`CPLEX Simplex - Primal Pricing Algorithm <CPLEX Simplex/ODH_XSimplex_-_Prim_Pric_Alg>`
   * - CPX_QPMAKEPSDIND
     - :doc:`CPLEX Quadratic - Adjust MIQP <CPLEX Quadratic/ODH_XQuadratic_-_Adjust_MIQP>`
   * - CPX_QPMETHOD
     - :doc:`CPLEX Quadratic - QP Method <CPLEX Quadratic/ODH_XQuadratic_-_QP_Method>`
   * - CPX_QPNZREADLIM
     - :doc:`CPLEX Quadratic - QP Nonzeros Read Limit <CPLEX Quadratic/ODH_XQuadratic_-_QP_Nonzeros_Read_Limit>`
   * - CPX_QTOLININD
     - :doc:`CPLEX Quadratic - QP Linearization <CPLEX Quadratic/ODH_XQuadratic_-_QP_Linearization>`
   * - CPX_RANDOMSEED
     - :doc:`CPLEX General - Random Seed <CPLEX General/ODH_XGeneral_-_Random_Seed>`
   * - CPX_REDUCE
     - :doc:`CPLEX Preprocessing - Preprocessing Reduction Types <CPLEX Preprocessing/ODH_XPrepr_-_Pre_reduction_types>`
   * - CPX_REINV
     - :doc:`CPLEX Simplex - Refactor <CPLEX Simplex/ODH_XSimplex_-_Refactor>`
   * - CPX_RELAXPREIND
     - :doc:`CPLEX MIP Preprocessing - Presolve Relaxed MIP <CPLEX MIP Preprocessing/ODH_XMIP_Prepr_-_Presolve_Re>`
   * - CPX_RELOBJDIF
     - :doc:`CPLEX MIP - Relative Difference Objective <CPLEX MIP/ODH_XMIP_-_Rel_Difference_Obj>`
   * - CPX_REPAIRTRIES
     - :doc:`CPLEX MIP - Number of Repair Attempts <CPLEX MIP/ODH_XMIP_-_NumberofRepairAttempts>`
   * - CPX_REPEATPRESOLVE
     - :doc:`CPLEX MIP Preprocessing - Repeat Presolve <CPLEX MIP Preprocessing/ODH_XMIP_Prepr_-_Repeat_Presolve>`
   * - CPX_RINSHEUR
     - :doc:`CPLEX MIP Heuristics - RINS Heuristic Frequency <CPLEX MIP Heuristics/ODH_XMIP_Heuristic_-_RINS_Heurist_Freq>`
   * - CPX_RLTCUTS
     - :doc:`CPLEX MIP Cuts - RLT Cuts <CPLEX MIP Cuts/ODH_XCuts_-_RLT_Cuts>`
   * - CPX_SCAIND
     - :doc:`CPLEX General - Scale <CPLEX General/ODH_XGeneral_-_Scale>`
   * - CPX_SIFTALG
     - :doc:`CPLEX General - Sifting Algorithm <CPLEX General/ODH_XGeneral_-_Sifting_Algorithm>`
   * - CPX_SIFTSIM
     - :doc:`CPLEX Simplex - Sifting from Simplex <CPLEX Simplex/ODH_XSimplex_-_Sifting_from_Simplex>`
   * - CPX_SIMDISPLAY
     - :doc:`CPLEX Logging - Simplex Display <CPLEX Logging/ODH_XLogging_-_Simplex_Display>`
   * - CPX_SINGLIM
     - :doc:`CPLEX Simplex - Singular <CPLEX Simplex/ODH_XSimplex_-_Singular>`
   * - CPX_SOLNPOOLAGAP
     - :doc:`CPLEX MIP Solution Pool - Pool Absolute Objective Gap <CPLEX MIP Solution Pool/ODH_XMIP_Solp_-_Pool_Abs_Obj_Gap>`
   * - CPX_SOLNPOOLCAPACITY
     - :doc:`CPLEX MIP Solution Pool - Pool Capacity <CPLEX MIP Solution Pool/ODH_XMIP_Solp_-_Pool_Capacity>`
   * - CPX_SOLNPOOLGAP
     - :doc:`CPLEX MIP Solution Pool - Pool Relative Objective Gap <CPLEX MIP Solution Pool/ODH_XMIP_Solp_-_Pool_Rel_Obj_Gap>`
   * - CPX_SOLNPOOLINTENSITY
     - :doc:`CPLEX MIP Solution Pool - Pool Intensity <CPLEX MIP Solution Pool/ODH_XMIP_Solp_-_Pool_Intensity>`
   * - CPX_SOLNPOOLREPLACE
     - :doc:`CPLEX MIP Solution Pool - Pool Replacement Strategy <CPLEX MIP Solution Pool/ODH_XMIP_Solp_-_Pool_Repl_Strat>`
   * - CPX_SOS1REFORM
     - :doc:`CPLEX MIP Preprocessing - SOS1 Reformulations <CPLEX MIP Preprocessing/ODH_XMIP_Prepr_-_SOS1_Reformulations>`
   * - CPX_SOS2REFORM
     - :doc:`CPLEX MIP Preprocessing - SOS2 Reformulations <CPLEX MIP Preprocessing/ODH_XMIP_Prepr_-_SOS2_Reformulations>`
   * - CPX_STARTALG
     - :doc:`CPLEX MIP - MIP Start Algorithm <CPLEX MIP/ODH_XMIP_-_MIP_Start_Algorit>`
   * - CPX_STRONGCANDLIM
     - :doc:`CPLEX MIP - MIP Candidate List <CPLEX MIP/ODH_XMIP_-_MIP_Cand_List>`
   * - CPX_STRONGITLIM
     - :doc:`CPLEX MIP - Number of Simplex Iterations <CPLEX MIP/ODH_XMIP_-_Nr_of_Simplex_Iter>`
   * - CPX_SUBALG
     - :doc:`CPLEX MIP - MIP Method <CPLEX MIP/ODH_XMIP_-_MIP_Method>`
   * - CPX_SUBMIPNODELIMIT
     - :doc:`CPLEX MIP Advanced - SubMIP Node Limit <CPLEX MIP Advanced/ODH_XMIP_Advanced_-_SubMIP_Node_Limit>`
   * - CPX_SUBMIPSCAIND
     - :doc:`CPLEX MIP Advanced - SubMIP Scale <CPLEX MIP Advanced/ODH_XMIP_Advanced_-_SubMIP_Scale>`
   * - CPX_SUBMIPSTARTALG
     - :doc:`CPLEX MIP Advanced - SubMIP Start Algorithm <CPLEX MIP Advanced/ODH_XMIP_Advanced_-_SubMIP_Start_Algorithm>`
   * - CPX_SUBMIPSUBALG
     - :doc:`CPLEX MIP Advanced - SubMIP Subproblem Algorithm <CPLEX MIP Advanced/ODH_XMIP_Advanced_-_SubMIP_Subproblem_Algorithm>`
   * - CPX_SYMMETRY
     - :doc:`CPLEX MIP Preprocessing - Preprocessing Symmetry <CPLEX MIP Preprocessing/ODH_XMIP_Prepr_-_Preproc_Sym>`
   * - CPX_THREADS
     - :doc:`CPLEX Parallel - Global Thread Limit <CPLEX Parallel/ODH_XPar_-_GlobalThreadLimit>`
   * - CPX_TRELIM
     - :doc:`CPLEX MIP - MIP Tree Memory Limit <CPLEX MIP/ODH_XMIP_-_MIP_Tree_Memory_Limit>`
   * - CPX_VARSEL
     - :doc:`CPLEX MIP - Select Variables <CPLEX MIP/ODH_XMIP_-_Select_Variables>`
   * - CPX_WORKMEM
     - :doc:`CPLEX MIP - Working Memory Limit <CPLEX MIP/ODH_XMIP_-_Working_Memory_Limit>`
   * - CPX_ZEROHALFCUTS
     - :doc:`CPLEX MIP Cuts - Zero Half Cuts <CPLEX MIP Cuts/ODH_XCuts_-_Zero_Half_Cuts>`


**Heuristic sub-model parameters** 

The heuristic sub-model parameters can only be set using a :doc:`ODH_-_Parameter_File`. The syntax for the parameters that influence the heuristic sub-model CPLEX solves is the following: SUB_<parameter> where <parameter> refers to the ODH-CPLEX name in the second table above. The syntax for the parameters that influence the heuristic sub-model CPLEX solves in Phase I is the following: PHASE1_<parameter>.



For example, SUB_CPX_RINSHEUR specifies the RINS heuristic frequency for CPLEX if it used to solve a heuristic sub-model, while PHASE1_CPX_RINSHEUR specifies the RINS heuristic frequency for CPLEX if it used to solve a heuristic sub-model in Phase I.



**Learn more about** 

*	:doc:`ODH_-_Parameter_File`
*	:doc:`General - Search Mode <General/ODH_General_-_Search_Mode>`  
