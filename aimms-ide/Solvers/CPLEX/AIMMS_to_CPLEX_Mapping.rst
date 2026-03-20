

.. _AIMMS_to_CPLEX_Mapping:


AIMMS to CPLEX Mapping
===========================

**Description** 

The table below shows in the left column the AIMMS CPLEX options; the middle column displays the CPLEX parameters that are associated with them. The right column displays the constants used in the CPLEX C API.

.. list-table::

   * - **Option name in AIMMS** 
     - **Name in CPLEX** 
     - **Name in CPLEX C API** 
   * - :doc:`Barrier - Barrier Algorithm <Barrier/CPLEX_Barrier_-_Barrier_Algorithm>`
     - Barrier algorithm
     - CPX_PARAM_BARALG
   * - :doc:`Barrier - Barrier Always <Barrier/CPLEX_Barrier_-_Barrier_Always>`
     - 
     - 
   * - :doc:`Barrier - Barrier Convergence Tolerance <Barrier/CPLEX_Barrier_-_Barrier_Convergence_>`
     - Barrier convergetol
     - CPX_PARAM_BAREPCOMP
   * - :doc:`Barrier - Barrier Crossover Algorithm <Barrier/CPLEX_Barrier_-_Barrier_cross>`
     - Barrier crossover
     - CPX_PARAM_BARCROSSALG
   * - :doc:`Barrier - Barrier Density Definition <Barrier/CPLEX_Barrier_-_Barrier_Density_Defi>`
     - Barrier colnonzeros
     - CPX_PARAM_BARCOLNZ
   * - :doc:`Barrier - Barrier Growth Limit <Barrier/CPLEX_Barrier_-_Barrier_Growth_Limit>`
     - Barrier limits growth
     - CPX_PARAM_BARGROWTH
   * - :doc:`Barrier - Barrier Iterations <Barrier/CPLEX_Barrier_-_Barrier_Iterations>`
     - Barrier limits iteration
     - CPX_PARAM_BARITLIM
   * - :doc:`Barrier - Barrier Maximal Number of Corrections <Barrier/CPLEX_Barrier_-_Barrier_Maximal_Numb>`
     - Barrier limits corrections
     - CPX_PARAM_BARMAXCOR
   * - :doc:`Barrier - Barrier Objective Range <Barrier/CPLEX_Barrier_-_Barrier_Objective_Ra>`
     - Barrier limits objrange
     - CPX_PARAM_BAROBJRNG
   * - :doc:`Barrier - Barrier Ordering <Barrier/CPLEX_Barrier_-_Barrier_Ordering>`
     - Barrier ordering
     - CPX_PARAM_BARORDER
   * - :doc:`Barrier - Barrier Progress Solution <Barrier/CPLEX_Barrier_-_Barrier_Prog_Sol>`
     - 
     - 
   * - :doc:`Barrier - Barrier Start Algorithm <Barrier/CPLEX_Barrier_-_Barrier_Start_Algori>`
     - Barrier startalg
     - CPX_PARAM_BARSTARTALG
   * - :doc:`Benders - Benders Decomposition Check Limit <Benders/CPLEX_Benders_-_Benders_Decomposition_Check_Limit>`
     - 
     - 
   * - :doc:`Benders - Benders Feasibility Cut Tolerance <Benders/CPLEX_Benders_-_Benders_Feasibility_Cut_Tolera>`
     - Benders tolerances feasibilitycut
     - CPX_PARAM_BENDERSFEASCUTTOL
   * - :doc:`Benders - Benders Optimality Cut Tolerance <Benders/CPLEX_Benders_-_Benders_Optimality_Cut_Toleran>`
     - Benders tolerances optimalitycut
     - CPX_PARAM_BENDERSOPTCUTTOL
   * - :doc:`Benders - Benders Strategy <Benders/CPLEX_Benders_-_Benders_Strategy>`
     - Benders strategy
     - CPX_PARAM_BENDERSSTRATEGY
   * - :doc:`Benders - Benders Worker Algorithm <Benders/CPLEX_Benders_-_Benders_Worker_Alg>`
     - Benders workeralgorithm
     - CPX_PARAM_WORKERALG
   * - :doc:`General - Advanced Start <General/CPLEX_General_-_AdvancedStart>`
     - Advance
     - CPX_PARAM_ADVIND
   * - :doc:`General - Check Solution <General/CPLEX_General_-_Check_Solution>`
     - 
     - 
   * - :doc:`General - Cleanup Coefficients <General/CPLEX_General_-_Cleanup_Coefficients>`
     - 
     - 
   * - :doc:`General - Clock Type <General/CPLEX_General_-_Clock_Type>`
     - Clocktype
     - CPX_PARAM_CLOCKTYPE
   * - :doc:`General - Cmd File <General/CPLEX_General_-_Cmd_File>`
     - 
     - 
   * - :doc:`General - Conflict Algorithm <General/CPLEX_General_-_Conflict_Algorithm>`
     - Conflict algorithm
     - CPX_PARAM_CONFLICTALG
   * - :doc:`General - Data Check and Modeling Assistance <General/CPLEX_General_-_Data_Check>`
     - Read datacheck
     - CPX_PARAM_DATACHECK
   * - :doc:`General - Deterministic Time Limit <General/CPLEX_General_-_Deterministic_Time_Limit>`
     - Dettimelimit
     - CPX_PARAM_DETTILIM
   * - :doc:`General - Display Solution Statistics <General/CPLEX_General_-_Display_Solution_Statistics>`
     - 
     - 
   * - :doc:`General - Farkas Infeasibility Proof <General/CPLEX_General_-_Farkas_Infeasibility_Proof>`
     - 
     - 
   * - :doc:`General - Feasopt Tolerance <General/CPLEX_General_-_Feasopt_tolerance>`
     - Feasopt tolerance
     - CPX_PARAM_Feasopt_Tolerance
   * - :doc:`General - LP File <General/CPLEX_General_-_LP_File>`
     - 
     - 
   * - :doc:`General - LP Method <General/CPLEX_General_-_LP_Method>`
     - Lpmethod
     - CPX_PARAM_LPMETHOD
   * - :doc:`General - Memory Emphasis <General/CPLEX_General_-_MemoryEmphasis>`
     - Emphasis memory
     - CPX_PARAM_MEMORYEMPHASIS
   * - :doc:`General - MPS <General/CPLEX_General_-_MPS>`
     - 
     - 
   * - :doc:`General - Numerical Emphasis <General/CPLEX_General_-_NumericalEmphasis>`
     - Emphasis numerical
     - CPX_PARAM_NUMERICALEMPHASIS
   * - :doc:`General - Ord File <General/CPLEX_General_-_Ord_File>`
     - 
     - 
   * - :doc:`General - Random Seed <General/CPLEX_General_-_Random_Seed>`
     - Randomseed
     - CPX_PARAM_RANDOMSEED
   * - :doc:`General - Read Parameter File <General/CPLEX_General_-_Read_Parameter_File>`
     - 
     - 
   * - :doc:`General - Restart <General/CPLEX_General_-_Restart>`
     - 
     - 
   * - :doc:`General - Restart File Number <General/CPLEX_General_-_Restart_File_Nr>`
     - 
     - 
   * - :doc:`General - Round Coefficients <General/CPLEX_General_-_Round_Coefficients>`
     - 
     - 
   * - :doc:`General - Sav File <General/CPLEX_General_-_Sav_File>`
     - 
     - 
   * - :doc:`General - Scale <General/CPLEX_General_-_Scale>`
     - Read scale
     - CPX_PARAM_SCAIND
   * - :doc:`General - Sensitivity Method <General/CPLEX_General_-_Sensitivity_Method>`
     - 
     - 
   * - :doc:`General - Sifting Algorithm <General/CPLEX_General_-_Sifting_Algorithm>`
     - Sifting algorithm
     - CPX_PARAM_SIFTALG
   * - :doc:`General - Solution File <General/CPLEX_General_-_Solution_File>`
     - 
     - 
   * - :doc:`General - Solution Type <General/CPLEX_General_-_Solution_Type>`
     - Solutiontype
     - CPX_PARAM_SOLUTIONTYPE
   * - :doc:`General - Stealth Mode <General/CPLEX_General_-_StealthMode>`
     - 
     - 
   * - :doc:`General - Unbounded Ray <General/CPLEX_General_-_Unbounded_Ray>`
     - 
     - 
   * - :doc:`General - Updates Batch Size <General/CPLEX_General_-_Updates_Batch_Size>`
     - 
     - 
   * - :doc:`General - Write Annotations File <General/CPLEX_General_-_Write_Annotations_File>`
     - 
     - 
   * - :doc:`General - Write Parameter File <General/CPLEX_General_-_Write_Parameter_File>`
     - 
     - 
   * - :doc:`Logging - Barrier Display <Logging/CPLEX_Logging_-_Barrier_Display>`
     - Barrier display
     - CPX_PARAM_BARDISPLAY
   * - :doc:`Logging - Clone Log Files <Logging/CPLEX_Logging_-_Clone_Log_Files>`
     - Output clonelog
     - CPX_PARAM_CLONELOG
   * - :doc:`Logging - MIP Display <Logging/CPLEX_Logging_-_MIP_Display>`
     - MIP display
     - CPX_PARAM_MIPDISPLAY
   * - :doc:`Logging - MIP Interval <Logging/CPLEX_Logging_-_MIP_Interval>`
     - MIP interval
     - CPX_PARAM_MIPINTERVAL
   * - :doc:`Logging - Multi Objective Display <Logging/CPLEX_Logging_-_Multi_Objective_Display>`
     - Multiobjective display 
     - CPX_PARAM_MULTIOBJDISPLAY
   * - :doc:`Logging - Parameter Display <Logging/CPLEX_Logging_-_Parameter_Display>`
     - Paramdisplay
     - CPX_PARAM_PARAMDISPLAY
   * - :doc:`Logging - Simplex Display <Logging/CPLEX_Logging_-_Simplex_Display>`
     - Simplex display
     - CPX_PARAM_SIMDISPLAY
   * - :doc:`Logging - Tuning Display <Logging/CPLEX_Logging_-_Tuning_Display>`
     - Tune display
     - CPX_PARAM_TUNINGDISPLAY
   * - :doc:`Logging - Backtrack <MIP/CPLEX_MIP_-_Backtrack>`
     - MIP strategy backtrack
     - CPX_PARAM_BTTOL
   * - :doc:`MIP - Branch <MIP/CPLEX_MIP_-_Branch>`
     - MIP strategy branch
     - CPX_PARAM_BRDIR
   * - :doc:`MIP - Difference Objective <MIP/CPLEX_MIP_-_Difference_Object>`
     - MIP tolerances objdifference
     - CPX_PARAM_OBJDIF
   * - :doc:`MIP - Integrality <MIP/CPLEX_MIP_-_Integrality>`
     - MIP tolerances integrality
     - CPX_PARAM_EPINT
   * - :doc:`MIP - Maximal Number of Nodes <MIP/CPLEX_MIP_-_Max_Nr_of_Nodes>`
     - MIP limits nodes
     - CPX_PARAM_NODELIM
   * - :doc:`MIP - MIP Basis <MIP/CPLEX_MIP_-_MIP_Basis>`
     - 
     - 
   * - :doc:`MIP - MIP Candidate List <MIP/CPLEX_MIP_-_MIP_Cand_List>`
     - MIP limits strongcand
     - CPX_PARAM_STRONGCANDLIM
   * - :doc:`MIP - MIP Dive Strategy <MIP/CPLEX_MIP_-_MIP_Dive_Strat>`
     - MIP strategy dive
     - CPX_PARAM_DIVETYPE
   * - :doc:`MIP - MIP Emphasis <MIP/CPLEX_MIP_-_MIP_Emphasis>`
     - Emphasis MIP
     - CPX_PARAM_MIPEMPHASIS
   * - :doc:`MIP - MIP Kappa <MIP/CPLEX_MIP_-_MIP_Kappa>`
     - MIP strategy kappastats
     - CPX_PARAM_MIPKAPPASTATS
   * - :doc:`MIP - MIP Method <MIP/CPLEX_MIP_-_MIP_Method>`
     - MIP strategy subalgorithm
     - CPX_PARAM_SUBALG
   * - :doc:`MIP - MIP Priority Order Switch <MIP/CPLEX_MIP_-_MIP_Priority_Order_Switch>`
     - MIP strategy order
     - CPX_PARAM_MIPORDIND
   * - :doc:`MIP - MIP Priority Order Type <MIP/CPLEX_MIP_-_MIP_Priority_Order_Type>`
     - MIP ordertype
     - CPX_PARAM_MIPORDTYPE
   * - :doc:`MIP - MIP Probing <MIP/CPLEX_MIP_-_MIP_Probing>`
     - MIP strategy probe
     - CPX_PARAM_PROBE
   * - :doc:`MIP - MIP Search Strategy <MIP/CPLEX_MIP_-_MIP_Search_Strategy>`
     - MIP strategy search
     - CPX_PARAM_MIPSEARCH
   * - :doc:`MIP - MIP Start Algorithm <MIP/CPLEX_MIP_-_MIP_Start_Algorit>`
     - MIP strategy startalgorithm
     - CPX_PARAM_STARTALG
   * - :doc:`MIP - MIP Tree Memory Limit <MIP/CPLEX_MIP_-_MIP_Tree_Memory_Limit>`
     - MIP limits treememory
     - CPX_PARAM_TRELIM
   * - :doc:`MIP - MIP Update <MIP/CPLEX_MIP_-_MIP_Update>`
     - 
     - 
   * - :doc:`MIP - Node File <MIP/CPLEX_MIP_-_Node_File>`
     - MIP strategy file
     - CPX_PARAM_NODEFILEIND
   * - :doc:`MIP - MIP Node Presolve <MIP/CPLEX_MIP_-_MIP_Node_Presolve>`
     - MIP strategy presolvenode
     - CPX_PARAM_PRESLVND
   * - :doc:`MIP - Number of Repair Attempts <MIP/CPLEX_MIP_-_NumberofRepairAttempts>`
     - MIP limits repairtries
     - CPX_PARAM_REPAIRTRIES
   * - :doc:`MIP - Number of Simplex Iterations <MIP/CPLEX_MIP_-_Nr_of_Simplex_Iter>`
     - MIP limits strongit
     - CPX_PARAM_STRONGITLIM
   * - :doc:`MIP - Probing Time <MIP/CPLEX_MIP_-_Probing_Time>`
     - MIP limits probetime
     - CPX_PARAM_PROBETIME
   * - :doc:`MIP - Probing Time Deterministic <MIP/CPLEX_MIP_-_Probing_Time_Deterministic>`
     - MIP limits probedettime
     - CPX_PARAM_PROBEDETTIME
   * - :doc:`MIP - Relative Difference Objective <MIP/CPLEX_MIP_-_Rel_Difference_Obj>`
     - MIP tolerances relobjdifference
     - CPX_PARAM_RELOBJDIF
   * - :doc:`MIP - Select Variables <MIP/CPLEX_MIP_-_Select_Variables>`
     - MIP strategy variableselect
     - CPX_PARAM_VARSEL
   * - :doc:`MIP - Selection of Nodes <MIP/CPLEX_MIP_-_Selection_of_Nodes>`
     - MIP strategy nodeselect
     - CPX_PARAM_NODESEL
   * - :doc:`MIP - Use Generic Callbacks <MIP/CPLEX_MIP_-_Use_Generic_Callbacks>`
     - 
     - 
   * - :doc:`MIP - Working Memory Limit <MIP/CPLEX_MIP_-_Working_Memory_Limit>`
     - Workmem
     - CPX_PARAM_WORKMEM
   * - :doc:`MIP - Write MIP Starts <MIP/CPLEX_MIP_-_Write_MIP_Starts>`
     - 
     - 
   * - :doc:`MIP Advanced - Find Fractional Root Solution <MIP Advanced/CPLEX_MIP_Advanced_-_Find_Fractional_Root_Solution>`
     - 
     - 
   * - :doc:`MIP Advanced - Lower Objective Stop <MIP Advanced/CPLEX_MIP_Advanced_-_Lower_Objective_Stop>`
     - MIP limits lowerobjstop
     - CPX_PARAM_LOWEROBJSTOP
   * - :doc:`MIP Advanced - SubMIP Node Limit <MIP Advanced/CPLEX_MIP_Advanced_-_SubMIP_Node_Limit>`
     - MIP submip nodelimit
     - CPX_PARAM_SUBMIPNODELIMIT
   * - :doc:`MIP Advanced - SubMIP Scale <MIP Advanced/CPLEX_MIP_Advanced_-_SubMIP_Scale>`
     - MIP submip scale
     - CPX_PARAM_SUBMIPSCAIND
   * - :doc:`MIP Advanced - SubMIP Start Algorithm <MIP Advanced/CPLEX_MIP_Advanced_-_SubMIP_Start_Algorithm>`
     - MIP submip startalg
     - CPX_PARAM_SUBMIPSTARTALG
   * - :doc:`MIP Advanced - SubMIP Subproblem Algorithm <MIP Advanced/CPLEX_MIP_Advanced_-_SubMIP_Subproblem_Algorithm>`
     - MIP submip subalg
     - CPX_PARAM_SUBMIPSUBALG
   * - :doc:`MIP Advanced - Upper Objective Stop <MIP Advanced/CPLEX_MIP_Advanced_-_Upper_Objective_Stop>`
     - MIP limits upperobjstop
     - CPX_PARAM_UPPEROBJSTOP
   * - :doc:`MIP Advanced - Write Cuts <MIP Advanced/CPLEX_MIP_Advanced_-_Write_Cuts>`
     - 
     - 
   * - :doc:`MIP Advanced - Write Cuts Variable Values <MIP Advanced/CPLEX_MIP_Advanced_-_Write_Cuts_Variable_Val>`
     - 
     - 
   * - :doc:`MIP Cuts - Bqp Cuts <MIP Cuts/CPLEX_Cuts_-_BQP_Cuts>`
     - MIP cuts bqp
     - CPX_PARAM_BQPCUTS
   * - :doc:`MIP Cuts - Clique Cuts <MIP Cuts/CPLEX_Cuts_-_Clique_Cuts>`
     - MIP cuts cliques
     - CPX_PARAM_CLIQUES
   * - :doc:`MIP Cuts - Cover Cuts <MIP Cuts/CPLEX_Cuts_-_Cover_Cuts>`
     - MIP cuts covers
     - CPX_PARAM_COVERS
   * - :doc:`MIP Cuts - Cut Generation Limit <MIP Cuts/CPLEX_Cuts_-_Cut_Gen_Limi>`
     - MIP limits aggforcut
     - CPX_PARAM_AGGCUTLIM
   * - :doc:`MIP Cuts - Cut Limit <MIP Cuts/CPLEX_Cuts_-_Cut_Limit>`
     - MIP limits eachcutlimit
     - CPX_PARAM_EACHCUTLIM
   * - :doc:`MIP Cuts - Cuts Factor <MIP Cuts/CPLEX_Cuts_-_Cuts_Factor>`
     - MIP limits cutsfactor
     - CPX_PARAM_CUTSFACTOR
   * - :doc:`MIP Cuts - Disjunctive Cuts <MIP Cuts/CPLEX_Cuts_-_Disjunct_Cuts>`
     - MIP cuts disjunctive
     - CPX_PARAM_DISJCUTS
   * - :doc:`MIP Cuts - Flow Cover Cuts <MIP Cuts/CPLEX_Cuts_-_Flow_Cover_Cuts>`
     - MIP cuts flow
     - CPX_PARAM_FLOWCOVERS
   * - :doc:`MIP Cuts - Flow Path Cuts <MIP Cuts/CPLEX_Cuts_-_Flow_Path_Cuts>`
     - MIP cuts pathcut
     - CPX_PARAM_FLOWPATHS
   * - :doc:`MIP Cuts - Gomory Cuts <MIP Cuts/CPLEX_Cuts_-_Gomory_Cuts>`
     - MIP cuts gomory
     - CPX_PARAM_FRACCUTS
   * - :doc:`MIP Cuts - Gomory Cuts Candidate Limit <MIP Cuts/CPLEX_Cuts_-_Gomory_Cuts_Cand>`
     - MIP limits gomorycand
     - CPX_PARAM_FRACCAND
   * - :doc:`MIP Cuts - Gomory Cuts Pass Limit <MIP Cuts/CPLEX_Cuts_-_Gomory_Cuts_Pass_L>`
     - MIP limits gomorypass
     - CPX_PARAM_FRACPASS
   * - :doc:`MIP Cuts - Gub Cover Cuts <MIP Cuts/CPLEX_Cuts_-_GUB_Cover_Cuts>`
     - MIP cuts gubcovers
     - CPX_PARAM_GUBCOVERS
   * - :doc:`MIP Cuts - Implied Bound Cuts <MIP Cuts/CPLEX_Cuts_-_Implied_Bound_Cuts>`
     - MIP cuts implied
     - CPX_PARAM_IMPLBD
   * - :doc:`MIP Cuts - Lift and Project Cuts <MIP Cuts/CPLEX_Cuts_-_Lift_and_Project_Cuts>`
     - MIP cuts liftproj
     - CPX_PARAM_LANDPCUTS
   * - :doc:`MIP Cuts - Local Implied Bound Cuts <MIP Cuts/CPLEX_Cuts_-_Local_Implied_Bound_Cuts>`
     - MIP cuts localimplied
     - CPX_PARAM_LOCALIMPLBD
   * - :doc:`MIP Cuts - MCF Cuts <MIP Cuts/CPLEX_Cuts_-_MCF_Cuts>`
     - MIP cuts mcfcut
     - CPX_PARAM_MCFCUTS
   * - :doc:`MIP Cuts - MIP Number of Cut Passes <MIP Cuts/CPLEX_Cuts_-_MIP_Nr_of_Cut_Pa>`
     - MIP limits cutpasses
     - CPX_PARAM_CUTPASS
   * - :doc:`MIP Cuts - Mixed Integer Rounding Cuts <MIP Cuts/CPLEX_Cuts_-_Mix_Integer_Round>`
     - MIP cuts mircut
     - CPX_PARAM_MIRCUTS
   * - :doc:`MIP Cuts - Node Cuts <MIP Cuts/CPLEX_Cuts_-_Node_cuts>`
     - MIP cuts nodecuts
     - CPX_PARAM_NODECUTS
   * - :doc:`MIP Cuts - RLT Cuts <MIP Cuts/CPLEX_Cuts_-_RLT_Cuts>`
     - MIP cuts rlt
     - CPX_PARAM_RLTCUTS
   * - :doc:`MIP Cuts - Zero Half Cuts <MIP Cuts/CPLEX_Cuts_-_Zero_Half_Cuts>`
     - MIP cuts zerohalf
     - CPX_PARAM_ZEROHALFCUTS
   * - :doc:`MIP Heuristics - Feasibility Pump Heuristic <MIP Heuristics/CPLEX_MIP_Heuristic_-_Feasibility_Pump_Heuristic>`
     - MIP strategy fpheur
     - CPX_PARAM_FPHEUR
   * - :doc:`MIP Heuristics - Heuristic Effort <MIP Heuristics/CPLEX_MIP_Heuristic_-_Heuristic_Effort>`
     - MIP strategy heuristiceffort
     - CPX_PARAM_HEUREFFORT
   * - :doc:`MIP Heuristics - Heuristic Frequency <MIP Heuristics/CPLEX_MIP_Heuristic_-_Heuristic_Freq>`
     - MIP strategy heuristicfreq
     - CPX_PARAM_HEURFREQ
   * - :doc:`MIP Heuristics - Local Branching Heuristic <MIP Heuristics/CPLEX_MIP_Heuristic_-_Local_Branch_Heur>`
     - MIP strategy lbheur
     - CPX_PARAM_LBHEUR
   * - :doc:`MIP Heuristics - RINS Heuristic Frequency <MIP Heuristics/CPLEX_MIP_Heuristic_-_RINS_Heurist_Freq>`
     - MIP strategy rinsheur
     - CPX_PARAM_RINSHEUR
   * - :doc:`MIP Preprocessing - Boundstrength <MIP Preprocessing/CPLEX_MIP_Prepr_-_Boundstreng>`
     - Preprocessing boundstrength
     - CPX_PARAM_BNDSTRENIND
   * - :doc:`MIP Preprocessing - Coefficient Reduction <MIP Preprocessing/CPLEX_MIP_Prepr_-_Coef_Reduc>`
     - Preprocessing coeffreduce
     - CPX_PARAM_COEREDIND
   * - :doc:`MIP Preprocessing - Preprocessing Symmetry <MIP Preprocessing/CPLEX_MIP_Prepr_-_Preproc_Sym>`
     - Preprocessing symmetry
     - CPX_PARAM_SYMMETRY
   * - :doc:`MIP Preprocessing - Presolve Relaxed MIP <MIP Preprocessing/CPLEX_MIP_Prepr_-_Presolve_Re>`
     - Preprocessing relax
     - CPX_PARAM_RELAXPREIND
   * - :doc:`MIP Preprocessing - Repeat Presolve <MIP Preprocessing/CPLEX_MIP_Prepr_-_Repeat_Presolve>`
     - Preprocessing repeatpresolve
     - CPX_PARAM_REPEATPRESOLVE
   * - :doc:`MIP Preprocessing - SOS1 Reformulations <MIP Preprocessing/CPLEX_MIP_Prepr_-_SOS1_Reformulations>`
     - Preprocessing sos1reform
     - CPX_PARAM_SOS1REFORM
   * - :doc:`MIP Preprocessing - SOS2 Reformulations <MIP Preprocessing/CPLEX_MIP_Prepr_-_SOS2_Reformulations>`
     - Preprocessing sos2reform
     - CPX_PARAM_SOS2REFORM
   * - :doc:`MIP Solution Polishing - Polishing Absolute MIP Gap <MIP Solution Polishing/CPLEX_Polishing_Absolute_MIP_Gap>`
     - MIP polishafter absmipgap
     - CPX_PARAM_POLISHAFTEREPAGAP
   * - :doc:`MIP Solution Polishing - Polishing Number of Nodes <MIP Solution Polishing/CPLEX_Polishing_Number_of_Nodes>`
     - MIP polishafter nodes
     - CPX_PARAM_POLISHAFTERNODE
   * - :doc:`MIP Solution Polishing - Polishing Number of Solutions <MIP Solution Polishing/CPLEX_Polishing_Number_of_Solutions>`
     - MIP polishafter solutions
     - CPX_PARAM_POLISHAFTERINTSOL
   * - :doc:`MIP Solution Polishing - Polishing Relative MIP Gap <MIP Solution Polishing/CPLEX_Polishing_Relative_MIP_Gap>`
     - MIP polishafter mipgap
     - CPX_PARAM_POLISHAFTEREPGAP
   * - :doc:`MIP Solution Polishing - Polishing Time <MIP Solution Polishing/CPLEX_Polishing_Time>`
     - MIP polishafter time
     - CPX_PARAM_POLISHAFTERTIME
   * - :doc:`MIP Solution Polishing - Polishing Time Deterministic <MIP Solution Polishing/CPLEX_Polishing_Time_Deterministic>`
     - MIP polishafter dettime
     - CPX_PARAM_POLISHAFTERDETTIME
   * - :doc:`MIP Solution Pool - Do Populate <MIP Solution Pool/CPLEX_MIP_Solp_-_Do_Populate>`
     - 
     - 
   * - :doc:`MIP Solution Pool - Pool Absolute Objective Gap <MIP Solution Pool/CPLEX_MIP_Solp_-_Pool_Abs_Obj_Gap>`
     - MIP pool absgap
     - CPX_PARAM_SOLNPOOLAGAP
   * - :doc:`MIP Solution Pool - Pool Capacity <MIP Solution Pool/CPLEX_MIP_Solp_-_Pool_Capacity>`
     - MIP pool capacity
     - CPX_PARAM_SOLNPOOLCAPACITY
   * - :doc:`MIP Solution Pool - Pool Intensity <MIP Solution Pool/CPLEX_MIP_Solp_-_Pool_Intensity>`
     - MIP pool intensity
     - CPX_PARAM_SOLNPOOLINTENSITY
   * - :doc:`MIP Solution Pool - Pool Relative Objective Gap <MIP Solution Pool/CPLEX_MIP_Solp_-_Pool_Rel_Obj_Gap>`
     - MIP pool relgap
     - CPX_PARAM_SOLNPOOLGAP
   * - :doc:`MIP Solution Pool - Pool Replacement Strategy <MIP Solution Pool/CPLEX_MIP_Solp_-_Pool_Repl_Strat>`
     - MIP pool replace
     - CPX_PARAM_SOLNPOOLREPLACE
   * - :doc:`MIP Solution Pool - Populate Time Limit <MIP Solution Pool/CPLEX_MIP_Solp_-_Populate_time_limit>`
     - 
     - 
   * - :doc:`MIP Solution Pool - Population Limit <MIP Solution Pool/CPLEX_MIP_Solp_-_Population_Limit>`
     - MIP limits populate
     - CPX_PARAM_POPULATELIM
   * - :doc:`Network - Network Extraction Level <Network/CPLEX_-_Network_Extraction_L>`
     - Network netfind
     - CPX_PARAM_NETFIND
   * - :doc:`Network - Network Feasibility <Network/CPLEX_-_Network_Feasibility>`
     - Network tolerances feasibility
     - CPX_PARAM_NETEPRHS
   * - :doc:`Network - Network Iterations <Network/CPLEX_-_Network_Iterations>`
     - Network iterations
     - CPX_PARAM_NETITLIM
   * - :doc:`Network - Network Optimality <Network/CPLEX_-_Network_Optimality>`
     - Network tolerances optimality
     - CPX_PARAM_NETEPOPT
   * - :doc:`Network - Network Pricing <Network/CPLEX_-_Network_Pricing>`
     - Network pricing
     - CPX_PARAM_NETPPRIIND
   * - :doc:`Parallel - Auxiliary Root Threads <Parallel/CPLEX_Par_-_Auxiliary_Root_Threads>`
     - MIP limits auxrootthreads
     - CPX_PARAM_AUXROOTTHREADS
   * - :doc:`Parallel - Global Thread Limit <Parallel/CPLEX_Par_-_GlobalThreadLimit>`
     - Threads
     - CPX_PARAM_THREADS
   * - :doc:`Parallel - Parallel Mode <Parallel/CPLEX_Par_-_Parallel_Mode>`
     - Parallel mode
     - CPX_PARAM_PARALLELMODE
   * - :doc:`Preprocessing - Aggregator <Preprocessing/CPLEX_Prepr_-_Aggregator>`
     - Preprocessing aggregator
     - CPX_PARAM_AGGIND
   * - :doc:`Preprocessing - Dependency <Preprocessing/CPLEX_Prepr_-_Dependency>`
     - Preprocessing dependency
     - CPX_PARAM_DEPIND
   * - :doc:`Preprocessing - Folding <Preprocessing/CPLEX_Prepr_-_Folding>`
     - Preprocessing folding
     - CPX_PARAM_FOLDING
   * - :doc:`Preprocessing - Limit Substitutions <Preprocessing/CPLEX_Prepr_-_Limit_Substitut>`
     - Preprocessing fill
     - CPX_PARAM_AGGFILL
   * - :doc:`Preprocessing - Number of Iterations in Presolve <Preprocessing/CPLEX_Prepr_-_Number_of_IterP>`
     - Preprocessing numpass
     - CPX_PARAM_PREPASS
   * - :doc:`Preprocessing - Preprocessing Reduction Types <Preprocessing/CPLEX_Prepr_-_Pre_reduction_types>`
     - Preprocessing reduce
     - CPX_PARAM_REDUCE
   * - :doc:`Preprocessing - Presolve <Preprocessing/CPLEX_Prepr_-_Presolve>`
     - Preprocessing presolve
     - CPX_PARAM_PREIND
   * - :doc:`Preprocessing - Presolve Pass Dual <Preprocessing/CPLEX_Prepr_-_Presolve_Pass_D>`
     - Preprocessing dual
     - CPX_PARAM_PREDUAL
   * - :doc:`Preprocessing - Print Presolve Status <Preprocessing/CPLEX_Prepr_-_Print_Prslv_Sta>`
     - 
     - 
   * - :doc:`QP - Adjust MIQP <QP/CPLEX_QP_-_Adjust_MIQP>`
     - Preprocessing qpmakepsd
     - CPX_PARAM_QPMAKEPSDIND
   * - :doc:`QP - Barrier Convergence Tolerance for QCP <QP/CPLEX_QP_-_Barrier_Conv_Toler>`
     - Bar qcpconvergetol
     - CPX_PARAM_BARQCPEPCOMP
   * - :doc:`QP - MIQCP Strategy <QP/CPLEX_QP_-_MIQCP_Strategy>`
     - MIP strategy miqcpstrat
     - CPX_PARAM_MIQCPSTRAT
   * - :doc:`QP - QCP Dual Values <QP/CPLEX_QP_-_QCP_Dual_Values>`
     - Preprocessing qcpduals
     - CPX_PARAM_CALCQCPDUALS
   * - :doc:`QP - QP Linearization <QP/CPLEX_QP_-_QP_Linearization>`
     - Preprocessing qtolin
     - CPX_PARAM_QTOLININD
   * - :doc:`QP - QP Method <QP/CPLEX_QP_-_QP_Method>`
     - Qpmethod
     - CPX_PARAM_QPMETHOD
   * - :doc:`QP - QP Nonzeros Read Limit <QP/CPLEX_QP_-_QP_Nonzeros_Read_Limit>`
     - Read qpnonzeros
     - CPX_PARAM_QPNZREADLIM
   * - :doc:`QP - Solution Target <QP/CPLEX_QP_-_Solution_Target>`
     - Optimalitytarget
     - CPX_PARAM_OPTIMALITYTARGET
   * - :doc:`Simplex - Crash Ordering <Simplex/CPLEX_Simplex_-_Crash_Ordering>`
     - Simplex crash
     - CPX_PARAM_CRAIND
   * - :doc:`Simplex - Dual Pricing Algorithm <Simplex/CPLEX_Simplex_-_Dual_Pric_Alg>`
     - Simplex dgradient
     - CPX_PARAM_DPRIIND
   * - :doc:`Simplex - Dynamic Row Management <Simplex/CPLEX_Simplex_-_Dynamic_Row_Management>`
     - simplex dynamicrows
     - CPX_PARAM_DYNAMICROWS
   * - :doc:`Simplex - Feasibility <Simplex/CPLEX_Simplex_-_Feasibility>`
     - Simplex tolerances feasibility
     - CPX_PARAM_EPRHS
   * - :doc:`Simplex - Markowitz <Simplex/CPLEX_Simplex_-_Markowitz>`
     - Simplex tolerances markowitz
     - CPX_PARAM_EPMRK
   * - :doc:`Simplex - Optimality <Simplex/CPLEX_Simplex_-_Optimality>`
     - Simplex tolerances optimality
     - CPX_PARAM_EPOPT
   * - :doc:`Simplex - Perturbation Constant <Simplex/CPLEX_Simplex_-_Perturb_Const>`
     - Simplex perturbationlimit
     - CPX_PARAM_EPPER
   * - :doc:`Simplex - Perturbation Indicator <Simplex/CPLEX_Simplex_-_Perturb_Indic>`
     - Simplex perturbationlimit
     - CPX_PARAM_PERIND
   * - :doc:`Simplex - Pricing <Simplex/CPLEX_Simplex_-_Pricing>`
     - Simplex pricing
     - CPX_PARAM_PRICELIM
   * - :doc:`Simplex - Primal Pricing Algorithm <Simplex/CPLEX_Simplex_-_Prim_Pric_Alg>`
     - Simplex pgradient
     - CPX_PARAM_PPRIIND
   * - :doc:`Simplex - Refactor <Simplex/CPLEX_Simplex_-_Refactor>`
     - Simplex refactor
     - CPX_PARAM_REINV
   * - :doc:`Simplex - Sifting from Simplex <Simplex/CPLEX_Simplex_-_Sifting_from_Simplex>`
     - Sifting simplex
     - CPX_PARAM_SIFTSIM
   * - :doc:`Simplex - Singular <Simplex/CPLEX_Simplex_-_Singular>`
     - Simplex limits singularity
     - CPX_PARAM_SINGLIM
   * - :doc:`Simplex - Stalled Iterations <Simplex/CPLEX_Simplex_-_Stalled_Iter>`
     - Simplex limits perturbation
     - CPX_PARAM_PERLIM
   * - :doc:`Tuning - Tuning Measure <Tuning/CPLEX_Tuning_-_Tuning_Measure>`
     - Tune measure
     - CPX_PARAM_TUNINGMEASURE
   * - :doc:`Tuning - Tuning Repeater <Tuning/CPLEX_Tuning_-_Tuning_Repeater>`
     - Tune repeat
     - CPX_PARAM_TUNINGREPEAT
   * - :doc:`Tuning - Tuning Time Limit <Tuning/CPLEX_Tuning_-_Tuning_Time_Limit>`
     - Tune timelimit
     - CPX_PARAM_TUNINGTILIM
   * - :doc:`Tuning - Tuning Time Limit Deterministic <Tuning/CPLEX_Tuning_-_Tuning_Time_Limit_Deter>`
     - Tune dettimelimit
     - CPX_PARAM_TUNINGDETTILIM


The table below shows Solvers General options that are mapped to CPLEX parameters.

.. list-table::

   * - **Option name in AIMMS**
     - **Name in CPLEX**
     - **Name in CPLEX C API**
   * - :doc:`MIP Options - Cutoff <../../Aimms/Options/Solvers General/MIP Options/MIP_Options_-_Cutoff>`
     - MIP tolerances lowercutoff
     - CPX_PARAM_CUTLO
   * - 
     - MIP tolerances uppercutoff
     - CPX_PARAM_CUTUP
   * - :doc:`MIP Options - Maximal Number of Integer Solutions <../../Aimms/Options/Solvers General/MIP Options/MIP_Options_-_Maximal_Number_o>`
     - MIP limits solutions
     - CPX_PARAM_INTSOLLIM
   * - :doc:`MIP Options - MIP Absolute Optimality Tolerance <../../Aimms/Options/Solvers General/MIP Options/MIP_Options_-_MIP_Absolute_Opt>`
     - MIP tolerances absmipgap
     - CPX_PARAM_EPAGAP
   * - :doc:`MIP Options - MIP Relative Optimality Tolerance <../../Aimms/Options/Solvers General/MIP Options/MIP_Options_-_MIP_Relative_Opt>`
     - MIP tolerances mipgap
     - CPX_PARAM_EPGAP
   * - :doc:`Stop Criteria - Iteration Limit <../../Aimms/Options/Solvers General/Stop Criteria/Stop_Criteria_-_Iteration_Limi>`
     - Simplex limits iterations
     - CPX_PARAM_ITLIM
   * - :doc:`Stop Criteria - Time Limit <../../Aimms/Options/Solvers General/Stop Criteria/Stop_Criteria_-_Time_Limit>`
     - Timelimit
     - CPX_PARAM_TILIM


