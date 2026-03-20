

.. _CPLEX_to_AIMMS_Mapping:


CPLEX to AIMMS Mapping
===========================

**Description** 

The table shows in the left column the parameters from CPLEX that can be set in AIMMS; the right column displays for each CPLEX parameter the associated AIMMS option.

.. list-table::
   :header-rows: 0

   * - **Name in CPLEX**
     - **Option name in AIMMS** 
   * - Advance
     - :doc:`General - Advanced Start <General/CPLEX_General_-_AdvancedStart>`
   * - Bar qcpconvergetol
     - :doc:`QP - Barrier Convergence Tolerance for QCP <QP/CPLEX_QP_-_Barrier_Conv_Toler>`
   * - Barrier algorithm
     - :doc:`Barrier - Barrier Algorithm <Barrier/CPLEX_Barrier_-_Barrier_Algorithm>`
   * - Barrier colnonzeros
     - :doc:`Barrier - Barrier Density Definition <Barrier/CPLEX_Barrier_-_Barrier_Density_Defi>`
   * - Barrier convergetol
     - :doc:`Barrier - Barrier Convergence Tolerance <Barrier/CPLEX_Barrier_-_Barrier_Convergence_>`
   * - Barrier crossover
     - :doc:`Barrier - Barrier Crossover Algorithm <Barrier/CPLEX_Barrier_-_Barrier_cross>`
   * - Barrier display
     - :doc:`Logging - Barrier Display <Logging/CPLEX_Logging_-_Barrier_Display>`
   * - Barrier limits corrections
     - :doc:`Barrier - Barrier Maximal Number of Corrections <Barrier/CPLEX_Barrier_-_Barrier_Maximal_Numb>`
   * - Barrier limits growth
     - :doc:`Barrier - Barrier Growth Limit <Barrier/CPLEX_Barrier_-_Barrier_Growth_Limit>`
   * - Barrier limits iteration
     - :doc:`Barrier - Barrier Iterations <Barrier/CPLEX_Barrier_-_Barrier_Iterations>`
   * - Barrier limits objrange
     - :doc:`Barrier - Barrier Objective Range <Barrier/CPLEX_Barrier_-_Barrier_Objective_Ra>`
   * - Barrier ordering
     - :doc:`Barrier - Barrier Ordering <Barrier/CPLEX_Barrier_-_Barrier_Ordering>`
   * - Barrier startalg
     - :doc:`Barrier - Barrier Start Algorithm <Barrier/CPLEX_Barrier_-_Barrier_Start_Algori>`
   * - Benders strategy
     - :doc:`Benders - Benders Strategy <Benders/CPLEX_Benders_-_Benders_Strategy>`
   * - Benders tolerances feasibilitycut
     - :doc:`Benders - Benders Feasibility Cut Tolerance <Benders/CPLEX_Benders_-_Benders_Feasibility_Cut_Tolera>`
   * - Benders tolerances optimalitycut
     - :doc:`Benders - Benders Optimality Cut Tolerance <Benders/CPLEX_Benders_-_Benders_Optimality_Cut_Toleran>`
   * - Benders workeralgorithm
     - :doc:`Benders - Benders Worker Algorithm <Benders/CPLEX_Benders_-_Benders_Worker_Alg>`
   * - Clocktype
     - :doc:`General - Clock Type <General/CPLEX_General_-_Clock_Type>`
   * - Conflict algorithm
     - :doc:`General - Conflict Algorithm <General/CPLEX_General_-_Conflict_Algorithm>`
   * - Dettimelimit
     - :doc:`General - Deterministic Time Limit <General/CPLEX_General_-_Deterministic_Time_Limit>`
   * - Emphasis memory
     - :doc:`General - Memory Emphasis <General/CPLEX_General_-_MemoryEmphasis>`
   * - Emphasis MIP
     - :doc:`MIP - MIP Emphasis <MIP/CPLEX_MIP_-_MIP_Emphasis>`
   * - Emphasis numerical
     - :doc:`General - Numerical Emphasis <General/CPLEX_General_-_NumericalEmphasis>`
   * - Feasopt tolerance
     - :doc:`General - Feasopt Tolerance <General/CPLEX_General_-_Feasopt_tolerance>`
   * - Lpmethod
     - :doc:`General - LP Method <General/CPLEX_General_-_LP_Method>`
   * - MIP cuts bqp
     - :doc:`MIP Cuts - Bqp Cuts <MIP Cuts/CPLEX_Cuts_-_BQP_Cuts>`
   * - MIP cuts cliques
     - :doc:`MIP Cuts - Clique Cuts <MIP Cuts/CPLEX_Cuts_-_Clique_Cuts>`
   * - MIP cuts covers
     - :doc:`MIP Cuts - Cover Cuts <MIP Cuts/CPLEX_Cuts_-_Cover_Cuts>`
   * - MIP cuts disjunctive
     - :doc:`MIP Cuts - Disjunctive Cuts <MIP Cuts/CPLEX_Cuts_-_Disjunct_Cuts>`
   * - MIP cuts flow
     - :doc:`MIP Cuts - Flow Cover Cuts <MIP Cuts/CPLEX_Cuts_-_Flow_Cover_Cuts>`
   * - MIP cuts gomory
     - :doc:`MIP Cuts - Gomory Cuts <MIP Cuts/CPLEX_Cuts_-_Gomory_Cuts>`
   * - MIP cuts gubcovers
     - :doc:`MIP Cuts - Gub Cover Cuts <MIP Cuts/CPLEX_Cuts_-_GUB_Cover_Cuts>`
   * - MIP cuts implied
     - :doc:`MIP Cuts - Implied Bound Cuts <MIP Cuts/CPLEX_Cuts_-_Implied_Bound_Cuts>`
   * - MIP cuts liftproj
     - :doc:`MIP Cuts - Lift and Project Cuts <MIP Cuts/CPLEX_Cuts_-_Lift_and_Project_Cuts>`
   * - MIP cuts localimplied
     - :doc:`MIP Cuts - Local Implied Bound Cuts <MIP Cuts/CPLEX_Cuts_-_Local_Implied_Bound_Cuts>`
   * - MIP cuts mcfcut
     - :doc:`MIP Cuts - MCF Cuts <MIP Cuts/CPLEX_Cuts_-_MCF_Cuts>`
   * - MIP cuts mircut
     - :doc:`MIP Cuts - Mixed Integer Rounding Cuts <MIP Cuts/CPLEX_Cuts_-_Mix_Integer_Round>`
   * - MIP cuts nodecuts
     - :doc:`MIP Cuts - Node Cuts <MIP Cuts/CPLEX_Cuts_-_Node_cuts>`
   * - MIP cuts pathcut
     - :doc:`MIP Cuts - Flow Path Cuts <MIP Cuts/CPLEX_Cuts_-_Flow_Path_Cuts>`
   * - MIP cuts rlt
     - :doc:`MIP Cuts - RLT Cuts <MIP Cuts/CPLEX_Cuts_-_RLT_Cuts>`
   * - MIP cuts zerohalf
     - :doc:`MIP Cuts - Zero Half Cuts <MIP Cuts/CPLEX_Cuts_-_Zero_Half_Cuts>`
   * - MIP display
     - :doc:`Logging - MIP Display <Logging/CPLEX_Logging_-_MIP_Display>`
   * - MIP interval
     - :doc:`Logging - MIP Interval <Logging/CPLEX_Logging_-_MIP_Interval>`
   * - MIP limits aggforcut
     - :doc:`MIP Cuts - Cut Generation Limit <MIP Cuts/CPLEX_Cuts_-_Cut_Gen_Limi>`
   * - MIP limits auxrootthreads
     - :doc:`Parallel - Auxiliary Root Threads <Parallel/CPLEX_Par_-_Auxiliary_Root_Threads>`
   * - MIP limits cutpasses
     - :doc:`MIP Cuts - MIP Number of Cut Passes <MIP Cuts/CPLEX_Cuts_-_MIP_Nr_of_Cut_Pa>`
   * - MIP limits cutsfactor
     - :doc:`MIP Cuts - Cuts Factor <MIP Cuts/CPLEX_Cuts_-_Cuts_Factor>`
   * - MIP limits eachcutlimit
     - :doc:`MIP Cuts - Cut Limit <MIP Cuts/CPLEX_Cuts_-_Cut_Limit>`
   * - MIP limits gomorycand
     - :doc:`MIP Cuts - Gomory Cuts Candidate Limit <MIP Cuts/CPLEX_Cuts_-_Gomory_Cuts_Cand>`
   * - MIP limits gomorypass
     - :doc:`MIP Cuts - Gomory Cuts Pass Limit <MIP Cuts/CPLEX_Cuts_-_Gomory_Cuts_Pass_L>`
   * - MIP limits lowerobjstop
     - :doc:`MIP Advanced - Lower Objective Stop <MIP Advanced/CPLEX_MIP_Advanced_-_Lower_Objective_Stop>`
   * - MIP limits nodes
     - :doc:`MIP - Maximal Number of Nodes <MIP/CPLEX_MIP_-_Max_Nr_of_Nodes>`
   * - MIP limits populate
     - :doc:`MIP Solution Pool - Population Limit <MIP Solution Pool/CPLEX_MIP_Solp_-_Population_Limit>`
   * - MIP limits probedettime
     - :doc:`MIP - Probing Time Deterministic <MIP/CPLEX_MIP_-_Probing_Time_Deterministic>`
   * - MIP limits probetime
     - :doc:`MIP - Probing Time <MIP/CPLEX_MIP_-_Probing_Time>`
   * - MIP limits repairtries
     - :doc:`MIP - Number of Repair Attempts <MIP/CPLEX_MIP_-_NumberofRepairAttempts>`
   * - MIP limits solutions
     - :doc:`MIP Options - Maximal Number of Integer Solutions <../../Aimms/Options/Solvers General/MIP Options/MIP_Options_-_Maximal_Number_o>`
   * - MIP limits strongcand
     - :doc:`MIP - MIP Candidate List <MIP/CPLEX_MIP_-_MIP_Cand_List>`
   * - MIP limits strongit
     - :doc:`MIP - Number of Simplex Iterations <MIP/CPLEX_MIP_-_Nr_of_Simplex_Iter>`
   * - MIP limits treememory
     - :doc:`MIP - MIP Tree Memory Limit <MIP/CPLEX_MIP_-_MIP_Tree_Memory_Limit>`
   * - MIP limits upperobjstop
     - :doc:`MIP Advanced - Upper Objective Stop <MIP Advanced/CPLEX_MIP_Advanced_-_Upper_Objective_Stop>`
   * - MIP ordertype
     - :doc:`MIP - MIP Priority Order Type <MIP/CPLEX_MIP_-_MIP_Priority_Order_Type>`
   * - MIP polishafter absmipgap
     - :doc:`MIP Solution Polishing - Polishing Absolute MIP Gap <MIP Solution Polishing/CPLEX_Polishing_Absolute_MIP_Gap>`
   * - MIP polishafter dettime
     - :doc:`MIP Solution Polishing - Polishing Time Deterministic <MIP Solution Polishing/CPLEX_Polishing_Time_Deterministic>`
   * - MIP polishafter mipgap
     - :doc:`MIP Solution Polishing - Polishing Relative MIP Gap <MIP Solution Polishing/CPLEX_Polishing_Relative_MIP_Gap>`
   * - MIP polishafter nodes
     - :doc:`MIP Solution Polishing - Polishing Number of Nodes <MIP Solution Polishing/CPLEX_Polishing_Number_of_Nodes>`
   * - MIP polishafter solutions
     - :doc:`MIP Solution Polishing - Polishing Number of Solutions <MIP Solution Polishing/CPLEX_Polishing_Number_of_Solutions>`
   * - MIP polishafter time
     - :doc:`MIP Solution Polishing - Polishing Time <MIP Solution Polishing/CPLEX_Polishing_Time>`
   * - MIP pool absgap
     - :doc:`MIP Solution Pool - Pool Absolute Objective Gap <MIP Solution Pool/CPLEX_MIP_Solp_-_Pool_Abs_Obj_Gap>`
   * - MIP pool capacity
     - :doc:`MIP Solution Pool - Pool Capacity <MIP Solution Pool/CPLEX_MIP_Solp_-_Pool_Capacity>`
   * - MIP pool intensity
     - :doc:`MIP Solution Pool - Pool Intensity <MIP Solution Pool/CPLEX_MIP_Solp_-_Pool_Intensity>`
   * - MIP pool relgap
     - :doc:`MIP Solution Pool - Pool Relative Objective Gap <MIP Solution Pool/CPLEX_MIP_Solp_-_Pool_Rel_Obj_Gap>`
   * - MIP pool replace
     - :doc:`MIP Solution Pool - Pool Replacement Strategy <MIP Solution Pool/CPLEX_MIP_Solp_-_Pool_Repl_Strat>`
   * - MIP strategy backtrack
     - :doc:`Logging - Backtrack <MIP/CPLEX_MIP_-_Backtrack>`
   * - MIP strategy branch
     - :doc:`MIP - Branch <MIP/CPLEX_MIP_-_Branch>`
   * - MIP strategy dive
     - :doc:`MIP - MIP Dive Strategy <MIP/CPLEX_MIP_-_MIP_Dive_Strat>`
   * - MIP strategy file
     - :doc:`MIP - Node File <MIP/CPLEX_MIP_-_Node_File>`
   * - MIP strategy fpheur
     - :doc:`MIP Heuristics - Feasibility Pump Heuristic <MIP Heuristics/CPLEX_MIP_Heuristic_-_Feasibility_Pump_Heuristic>`
   * - MIP strategy heuristiceffort
     - :doc:`MIP Heuristics - Heuristic Effort <MIP Heuristics/CPLEX_MIP_Heuristic_-_Heuristic_Effort>`
   * - MIP strategy heuristicfreq
     - :doc:`MIP Heuristics - Heuristic Frequency <MIP Heuristics/CPLEX_MIP_Heuristic_-_Heuristic_Freq>`
   * - MIP strategy kappastats
     - :doc:`MIP - MIP Kappa <MIP/CPLEX_MIP_-_MIP_Kappa>`
   * - MIP strategy lbheur
     - :doc:`MIP Heuristics - Local Branching Heuristic <MIP Heuristics/CPLEX_MIP_Heuristic_-_Local_Branch_Heur>`
   * - MIP strategy miqcpstrat
     - :doc:`QP - MIQCP Strategy <QP/CPLEX_QP_-_MIQCP_Strategy>`
   * - MIP strategy nodeselect
     - :doc:`MIP - Selection of Nodes <MIP/CPLEX_MIP_-_Selection_of_Nodes>`
   * - MIP strategy order
     - :doc:`MIP - MIP Priority Order Switch <MIP/CPLEX_MIP_-_MIP_Priority_Order_Switch>`
   * - MIP strategy presolvenode
     - :doc:`MIP - MIP Node Presolve <MIP/CPLEX_MIP_-_MIP_Node_Presolve>`
   * - MIP strategy probe
     - :doc:`MIP - MIP Probing <MIP/CPLEX_MIP_-_MIP_Probing>`
   * - MIP strategy rinsheur
     - :doc:`MIP Heuristics - RINS Heuristic Frequency <MIP Heuristics/CPLEX_MIP_Heuristic_-_RINS_Heurist_Freq>`
   * - MIP strategy search
     - :doc:`MIP - MIP Search Strategy <MIP/CPLEX_MIP_-_MIP_Search_Strategy>`
   * - MIP strategy startalgorithm
     - :doc:`MIP - MIP Start Algorithm <MIP/CPLEX_MIP_-_MIP_Start_Algorit>`
   * - MIP strategy subalgorithm
     - :doc:`MIP - MIP Method <MIP/CPLEX_MIP_-_MIP_Method>`
   * - MIP strategy variableselect
     - :doc:`MIP - Select Variables <MIP/CPLEX_MIP_-_Select_Variables>`
   * - MIP submip nodelimit
     - :doc:`MIP Advanced - SubMIP Node Limit <MIP Advanced/CPLEX_MIP_Advanced_-_SubMIP_Node_Limit>`
   * - MIP submip scale
     - :doc:`MIP Advanced - SubMIP Scale <MIP Advanced/CPLEX_MIP_Advanced_-_SubMIP_Scale>`
   * - MIP submip startalg
     - :doc:`MIP Advanced - SubMIP Start Algorithm <MIP Advanced/CPLEX_MIP_Advanced_-_SubMIP_Start_Algorithm>`
   * - MIP submip subalg
     - :doc:`MIP Advanced - SubMIP Subproblem Algorithm <MIP Advanced/CPLEX_MIP_Advanced_-_SubMIP_Subproblem_Algorithm>`
   * - MIP tolerances absmipgap
     - :doc:`MIP Options - MIP Absolute Optimality Tolerance <../../Aimms/Options/Solvers General/MIP Options/MIP_Options_-_MIP_Absolute_Opt>`
   * - MIP tolerances integrality
     - :doc:`MIP - Integrality <MIP/CPLEX_MIP_-_Integrality>`
   * - MIP tolerances lowercutoff
     - :doc:`MIP Options - Cutoff <../../Aimms/Options/Solvers General/MIP Options/MIP_Options_-_Cutoff>`
   * - MIP tolerances mipgap
     - :doc:`MIP Options - MIP Relative Optimality Tolerance <../../Aimms/Options/Solvers General/MIP Options/MIP_Options_-_MIP_Relative_Opt>`
   * - MIP tolerances objdifference
     - :doc:`MIP - Difference Objective <MIP/CPLEX_MIP_-_Difference_Object>`
   * - MIP tolerances relobjdifference
     - :doc:`MIP - Relative Difference Objective <MIP/CPLEX_MIP_-_Rel_Difference_Obj>`
   * - MIP tolerances uppercutoff
     - :doc:`MIP Options - Cutoff <../../Aimms/Options/Solvers General/MIP Options/MIP_Options_-_Cutoff>`
   * - Multiobjective display
     - :doc:`Logging - Multi Objective Display <Logging/CPLEX_Logging_-_Multi_Objective_Display>`
   * - Network iterations
     - :doc:`Network - Network Iterations <Network/CPLEX_-_Network_Iterations>`
   * - Network netfind
     - :doc:`Network - Network Extraction Level <Network/CPLEX_-_Network_Extraction_L>`
   * - Network pricing
     - :doc:`Network - Network Pricing <Network/CPLEX_-_Network_Pricing>`
   * - Network tolerances feasibility
     - :doc:`Network - Network Feasibility <Network/CPLEX_-_Network_Feasibility>`
   * - Network tolerances optimality
     - :doc:`Network - Network Optimality <Network/CPLEX_-_Network_Optimality>`
   * - Optimalitytarget
     - :doc:`QP - Solution Target <QP/CPLEX_QP_-_Solution_Target>`
   * - Output clonelog
     - :doc:`Logging - Clone Log Files <Logging/CPLEX_Logging_-_Clone_Log_Files>`
   * - Parallel mode
     - :doc:`Parallel - Parallel Mode <Parallel/CPLEX_Par_-_Parallel_Mode>`
   * - Paramdisplay
     - :doc:`Logging - Parameter Display <Logging/CPLEX_Logging_-_Parameter_Display>`
   * - Preprocessing aggregator
     - :doc:`Preprocessing - Aggregator <Preprocessing/CPLEX_Prepr_-_Aggregator>`
   * - Preprocessing boundstrength
     - :doc:`MIP Preprocessing - Boundstrength <MIP Preprocessing/CPLEX_MIP_Prepr_-_Boundstreng>`
   * - Preprocessing coeffreduce
     - :doc:`MIP Preprocessing - Coefficient Reduction <MIP Preprocessing/CPLEX_MIP_Prepr_-_Coef_Reduc>`
   * - Preprocessing dependency
     - :doc:`Preprocessing - Dependency <Preprocessing/CPLEX_Prepr_-_Dependency>`
   * - Preprocessing dual
     - :doc:`Preprocessing - Presolve Pass Dual <Preprocessing/CPLEX_Prepr_-_Presolve_Pass_D>`
   * - Preprocessing fill
     - :doc:`Preprocessing - Limit Substitutions <Preprocessing/CPLEX_Prepr_-_Limit_Substitut>`
   * - Preprocessing folding
     - :doc:`Preprocessing - Folding <Preprocessing/CPLEX_Prepr_-_Folding>`
   * - Preprocessing numpass
     - :doc:`Preprocessing - Number of Iterations in Presolve <Preprocessing/CPLEX_Prepr_-_Number_of_IterP>`
   * - Preprocessing presolve
     - :doc:`Preprocessing - Presolve <Preprocessing/CPLEX_Prepr_-_Presolve>`
   * - Preprocessing qcpduals
     - :doc:`QP - QCP Dual Values <QP/CPLEX_QP_-_QCP_Dual_Values>`
   * - Preprocessing qpmakepsd
     - :doc:`QP - Adjust MIQP <QP/CPLEX_QP_-_Adjust_MIQP>`
   * - Preprocessing qtolin
     - :doc:`QP - QP Linearization <QP/CPLEX_QP_-_QP_Linearization>`
   * - Preprocessing reduce
     - :doc:`Preprocessing - Preprocessing Reduction Types <Preprocessing/CPLEX_Prepr_-_Pre_reduction_types>`
   * - Preprocessing relax
     - :doc:`MIP Preprocessing - Presolve Relaxed MIP <MIP Preprocessing/CPLEX_MIP_Prepr_-_Presolve_Re>`
   * - Preprocessing repeatpresolve
     - :doc:`MIP Preprocessing - Repeat Presolve <MIP Preprocessing/CPLEX_MIP_Prepr_-_Repeat_Presolve>`
   * - Preprocessing sos1reform
     - :doc:`MIP Preprocessing - SOS1 Reformulations <MIP Preprocessing/CPLEX_MIP_Prepr_-_SOS1_Reformulations>`
   * - Preprocessing sos2reform
     - :doc:`MIP Preprocessing - SOS2 Reformulations <MIP Preprocessing/CPLEX_MIP_Prepr_-_SOS2_Reformulations>`
   * - Preprocessing symmetry
     - :doc:`MIP Preprocessing - Preprocessing Symmetry <MIP Preprocessing/CPLEX_MIP_Prepr_-_Preproc_Sym>`
   * - QPMethod
     - :doc:`QP - QP Method <QP/CPLEX_QP_-_QP_Method>`
   * - Randomseed
     - :doc:`General - Random Seed <General/CPLEX_General_-_Random_Seed>`
   * - Read datacheck
     - :doc:`General - Data Check and Modeling Assistance <General/CPLEX_General_-_Data_Check>`
   * - Read qpnonzeros
     - :doc:`QP - QP Nonzeros Read Limit <QP/CPLEX_QP_-_QP_Nonzeros_Read_Limit>`
   * - Read scale
     - :doc:`General - Scale <General/CPLEX_General_-_Scale>`
   * - Sifting algorithm
     - :doc:`General - Sifting Algorithm <General/CPLEX_General_-_Sifting_Algorithm>`
   * - Sifting simplex
     - :doc:`Simplex - Sifting from Simplex <Simplex/CPLEX_Simplex_-_Sifting_from_Simplex>`
   * - Simplex crash
     - :doc:`Simplex - Crash Ordering <Simplex/CPLEX_Simplex_-_Crash_Ordering>`
   * - Simplex dgradient
     - :doc:`Simplex - Dual Pricing Algorithm <Simplex/CPLEX_Simplex_-_Dual_Pric_Alg>`
   * - Simplex display
     - :doc:`Logging - Simplex Display <Logging/CPLEX_Logging_-_Simplex_Display>`
   * - Simplex dynamicrows
     - :doc:`Simplex - Dynamic Row Management <Simplex/CPLEX_Simplex_-_Dynamic_Row_Management>`
   * - Simplex limits iterations
     - :doc:`Stop Criteria - Iteration Limit <../../Aimms/Options/Solvers General/Stop Criteria/Stop_Criteria_-_Iteration_Limi>`
   * - Simplex limits perturbation
     - :doc:`Simplex - Stalled Iterations <Simplex/CPLEX_Simplex_-_Stalled_Iter>`
   * - Simplex limits singularity
     - :doc:`Simplex - Singular <Simplex/CPLEX_Simplex_-_Singular>`
   * - Simplex perturbationlimit
     - :doc:`Simplex - Perturbation Constant <Simplex/CPLEX_Simplex_-_Perturb_Const>`
   * - Simplex perturbationlimit
     - :doc:`Simplex - Perturbation Indicator <Simplex/CPLEX_Simplex_-_Perturb_Indic>`
   * - Simplex pgradient
     - :doc:`Simplex - Primal Pricing Algorithm <Simplex/CPLEX_Simplex_-_Prim_Pric_Alg>`
   * - Simplex pricing
     - :doc:`Simplex - Pricing <Simplex/CPLEX_Simplex_-_Pricing>`
   * - Simplex refactor
     - :doc:`Simplex - Refactor <Simplex/CPLEX_Simplex_-_Refactor>`
   * - Simplex tolerances feasibility
     - :doc:`Simplex - Feasibility <Simplex/CPLEX_Simplex_-_Feasibility>`
   * - Simplex tolerances markowitz
     - :doc:`Simplex - Markowitz <Simplex/CPLEX_Simplex_-_Markowitz>`
   * - Simplex tolerances optimality
     - :doc:`Simplex - Optimality <Simplex/CPLEX_Simplex_-_Optimality>`
   * - Solutiontype
     - :doc:`General - Solution Type <General/CPLEX_General_-_Solution_Type>`
   * - Threads
     - :doc:`Parallel - Global Thread Limit <Parallel/CPLEX_Par_-_GlobalThreadLimit>`
   * - Timelimit
     - :doc:`Stop Criteria - Time Limit <../../Aimms/Options/Solvers General/Stop Criteria/Stop_Criteria_-_Time_Limit>`
   * - Tune dettimelimit
     - :doc:`Tuning - Tuning Time Limit Deterministic <Tuning/CPLEX_Tuning_-_Tuning_Time_Limit_Deter>`
   * - Tune display
     - :doc:`Logging - Tuning Display <Logging/CPLEX_Logging_-_Tuning_Display>`
   * - Tune measure
     - :doc:`Tuning - Tuning Measure <Tuning/CPLEX_Tuning_-_Tuning_Measure>`
   * - Tune repeat
     - :doc:`Tuning - Tuning Repeater <Tuning/CPLEX_Tuning_-_Tuning_Repeater>`
   * - Tune timelimit
     - :doc:`Tuning - Tuning Time Limit <Tuning/CPLEX_Tuning_-_Tuning_Time_Limit>`
   * - Workmem
     - :doc:`MIP - Working Memory Limit <MIP/CPLEX_MIP_-_Working_Memory_Limit>`
