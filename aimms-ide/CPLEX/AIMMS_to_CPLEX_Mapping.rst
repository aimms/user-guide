

.. _AIMMS_to_CPLEX_22_1_Mapping:
.. _CPLEX_AIMMS_to_CPLEX_22_1_Mapping:


AIMMS to CPLEX 22.1 Mapping
===========================

**Description** 

The table below shows in the left column the AIMMS CPLEX 22.1 options; the middle column displays the CPLEX 22.1 parameters that are associated with them. The right column displays the constants used in the CPLEX C API.




.. list-table::

   * - **Option name in AIMMS** 
     - **Name in CPLEX** 
     - **Name in CPLEX C API** 
   * - :ref:`CPLEX_Barrier_-_Barrier_Algorithm`  
     - Barrier algorithm
     - CPX_PARAM_BARALG
   * - :ref:`CPLEX_Barrier_-_Barrier_Always`  
     - 
     - 
   * - :ref:`CPLEX_Barrier_-_Barrier_Convergence_`  
     - Barrier convergetol
     - CPX_PARAM_BAREPCOMP
   * - :ref:`CPLEX_Barrier_-_Barrier_cross` 
     - Barrier crossover
     - CPX_PARAM_BARCROSSALG
   * - :ref:`CPLEX_Barrier_-_Barrier_Density_Defi`  
     - Barrier colnonzeros
     - CPX_PARAM_BARCOLNZ
   * - :ref:`CPLEX_Barrier_-_Barrier_Growth_Limit`  
     - Barrier limits growth
     - CPX_PARAM_BARGROWTH
   * - :ref:`CPLEX_Barrier_-_Barrier_Iterations`  
     - Barrier limits iteration
     - CPX_PARAM_BARITLIM
   * - :ref:`CPLEX_Barrier_-_Barrier_Maximal_Numb`  
     - Barrier limits corrections
     - CPX_PARAM_BARMAXCOR
   * - :ref:`CPLEX_Barrier_-_Barrier_Objective_Ra`  
     - Barrier limits objrange
     - CPX_PARAM_BAROBJRNG
   * - :ref:`CPLEX_Barrier_-_Barrier_Ordering`  
     - Barrier ordering
     - CPX_PARAM_BARORDER
   * - :ref:`CPLEX_Barrier_-_Barrier_Prog_Sol` 
     - 
     - 
   * - :ref:`CPLEX_Barrier_-_Barrier_Start_Algori`  
     - Barrier startalg	
     - CPX_PARAM_BARSTARTALG
   * - :ref:`CPLEX_Benders_-_Benders_Decomposition_Check_Limit` 
     - 
     - 
   * - :ref:`CPLEX_Benders_-_Benders_Feasibility_Cut_Tolera` 
     - Benders tolerances feasibilitycut
     - CPX_PARAM_BENDERSFEASCUTTOL
   * - :ref:`CPLEX_Benders_-_Benders_Optimality_Cut_Toleran` 
     - Benders tolerances optimalitycut
     - CPX_PARAM_BENDERSOPTCUTTOL
   * - :ref:`CPLEX_Benders_-_Benders_Strategy` 
     - Benders strategy
     - CPX_PARAM_BENDERSSTRATEGY
   * - :ref:`CPLEX_Benders_-_Benders_Worker_Alg` 
     - Benders workeralgorithm
     - CPX_PARAM_WORKERALG
   * - :ref:`CPLEX_General_-_AdvancedStart` 
     - Advance
     - CPX_PARAM_ADVIND
   * - :ref:`CPLEX_General_-_Check_Solution` 
     - 
     - 
   * - :ref:`CPLEX_General_-_Cleanup_Coefficients` 
     - 
     - 
   * - :ref:`CPLEX_General_-_Clock_Type` 
     - Clocktype
     - CPX_PARAM_CLOCKTYPE
   * - :ref:`CPLEX_General_-_Cmd_File`  
     - 
     - 
   * - :ref:`CPLEX_General_-_Conflict_Algorithm`  
     - Conflict algorithm
     - CPX_PARAM_CONFLICTALG
   * - :ref:`CPLEX_General_-_Data_Check`  
     - Read datacheck
     - CPX_PARAM_DATACHECK
   * - :ref:`CPLEX_General_-_Deterministic_Time_Limit` 
     - Dettimelimit
     - CPX_PARAM_DETTILIM
   * - :ref:`CPLEX_General_-_Display_Solution_Statistics`  
     - 
     - 
   * - :ref:`CPLEX_General_-_Farkas_Infeasibility_Proof`  
     - 
     - 
   * - :ref:`CPLEX_General_-_Feasopt_tolerance` 
     - Feasopt tolerance
     - CPX_PARAM_Feasopt_Tolerance
   * - :ref:`CPLEX_General_-_LP_File`  
     - 
     - 
   * - :ref:`CPLEX_General_-_LP_Method`  
     - Lpmethod
     - CPX_PARAM_LPMETHOD
   * - :ref:`CPLEX_General_-_MemoryEmphasis` 
     - Emphasis memory
     - CPX_PARAM_MEMORYEMPHASIS
   * - :ref:`CPLEX_General_-_MPS`  
     - 
     - 
   * - :ref:`CPLEX_General_-_NumericalEmphasis` 
     - Emphasis numerical
     - CPX_PARAM_NUMERICALEMPHASIS
   * - :ref:`CPLEX_General_-_Ord_File`  
     - 
     - 
   * - :ref:`CPLEX_General_-_Random_Seed`  
     - Randomseed
     - CPX_PARAM_RANDOMSEED
   * - :ref:`CPLEX_General_-_Read_Parameter_File`  
     - 
     - 
   * - :ref:`CPLEX_General_-_Restart`  
     - 
     - 
   * - :ref:`CPLEX_General_-_Restart_File_Nr` 
     - 
     - 
   * - :ref:`CPLEX_General_-_Round_Coefficients` 
     - 
     - 
   * - :ref:`CPLEX_General_-_Sav_File`  
     - 
     - 
   * - :ref:`CPLEX_General_-_Scale`  
     - Read scale
     - CPX_PARAM_SCAIND
   * - :ref:`CPLEX_General_-_Sensitivity_Method`  
     - 
     - 
   * - :ref:`CPLEX_General_-_Sifting_Algorithm`  
     - Sifting algorithm
     - CPX_PARAM_SIFTALG
   * - :ref:`CPLEX_General_-_Solution_File`  
     - 
     - 
   * - :ref:`CPLEX_General_-_Solution_Type`  
     - Solutiontype
     - CPX_PARAM_SOLUTIONTYPE
   * - :ref:`CPLEX_General_-_StealthMode`  
     - 
     - 
   * - :ref:`CPLEX_General_-_Unbounded_Ray`  
     - 
     - 
   * - :ref:`CPLEX_General_-_Updates_Batch_Size`  
     - 
     - 
   * - :ref:`CPLEX_General_-_Write_Annotations_File`  
     - 
     - 
   * - :ref:`CPLEX_General_-_Write_Parameter_File`  
     - 
     - 
   * - :ref:`CPLEX_Logging_-_Barrier_Display`  
     - Barrier display
     - CPX_PARAM_BARDISPLAY
   * - :ref:`CPLEX_Logging_-_Clone_Log_Files` 
     - Output clonelog
     - CPX_PARAM_CLONELOG
   * - :ref:`CPLEX_Logging_-_MIP_Display`  
     - MIP display
     - CPX_PARAM_MIPDISPLAY
   * - :ref:`CPLEX_Logging_-_MIP_Interval` 
     - MIP interval
     - CPX_PARAM_MIPINTERVAL
   * - :ref:`CPLEX_Logging_-_Multi_Objective_Display` 
     - Multiobjective display 
     - CPX_PARAM_MULTIOBJDISPLAY
   * - :ref:`CPLEX_Logging_-_Parameter_Display` 
     - Paramdisplay
     - CPX_PARAM_PARAMDISPLAY
   * - :ref:`CPLEX_Logging_-_Simplex_Display`  
     - Simplex display
     - CPX_PARAM_SIMDISPLAY
   * - :ref:`CPLEX_Logging_-_Tuning_Display` 
     - Tune display
     - CPX_PARAM_TUNINGDISPLAY
   * - :ref:`CPLEX_MIP_-_Backtrack`  
     - MIP strategy backtrack
     - CPX_PARAM_BTTOL
   * - :ref:`CPLEX_MIP_-_Branch`  
     - MIP strategy branch
     - CPX_PARAM_BRDIR
   * - :ref:`CPLEX_MIP_-_Difference_Object`  
     - MIP tolerances objdifference
     - CPX_PARAM_OBJDIF
   * - :ref:`CPLEX_MIP_-_Integrality`  
     - MIP tolerances integrality
     - CPX_PARAM_EPINT
   * - :ref:`CPLEX_MIP_-_Max_Nr_of_Nodes`  
     - MIP limits nodes
     - CPX_PARAM_NODELIM
   * - :ref:`CPLEX_MIP_-_MIP_Basis`  
     - 
     - 
   * - :ref:`CPLEX_MIP_-_MIP_Cand_List` 
     - MIP limits strongcand
     - CPX_PARAM_STRONGCANDLIM
   * - :ref:`CPLEX_MIP_-_MIP_Dive_Strat`  
     - MIP strategy dive	
     - CPX_PARAM_DIVETYPE
   * - :ref:`CPLEX_MIP_-_MIP_Emphasis` 
     - Emphasis MIP
     - CPX_PARAM_MIPEMPHASIS
   * - :ref:`CPLEX_MIP_-_MIP_Kappa`  
     - MIP strategy kappastats
     - CPX_PARAM_MIPKAPPASTATS
   * - :ref:`CPLEX_MIP_-_MIP_Method`  
     - MIP strategy subalgorithm
     - CPX_PARAM_SUBALG
   * - :ref:`CPLEX_MIP_-_MIP_Priority_Order_Switch` 
     - MIP strategy order
     - CPX_PARAM_MIPORDIND
   * - :ref:`CPLEX_MIP_-_MIP_Priority_Order_Type` 
     - MIP ordertype
     - CPX_PARAM_MIPORDTYPE
   * - :ref:`CPLEX_MIP_-_MIP_Probing` 
     - MIP strategy probe
     - CPX_PARAM_PROBE
   * - :ref:`CPLEX_MIP_-_MIP_Search_Strategy` 
     - MIP strategy search
     - CPX_PARAM_MIPSEARCH
   * - :ref:`CPLEX_MIP_-_MIP_Start_Algorit`  
     - MIP strategy startalgorithm
     - CPX_PARAM_STARTALG
   * - :ref:`CPLEX_MIP_-_MIP_Tree_Memory_Limit`  
     - MIP limits treememory
     - CPX_PARAM_TRELIM
   * - :ref:`CPLEX_MIP_-_MIP_Update`  
     - 
     - 
   * - :ref:`CPLEX_MIP_-_Node_File`  
     - MIP strategy file
     - CPX_PARAM_NODEFILEIND
   * - :ref:`CPLEX_MIP_-_MIP_Node_Presolve`  
     - MIP strategy presolvenode
     - CPX_PARAM_PRESLVND
   * - :ref:`CPLEX_MIP_-_NumberofRepairAttempts` 
     - MIP limits repairtries
     - CPX_PARAM_REPAIRTRIES
   * - :ref:`CPLEX_MIP_-_Nr_of_Simplex_Iter` 
     - MIP limits strongit
     - CPX_PARAM_STRONGITLIM
   * - :ref:`CPLEX_MIP_-_Probing_Time`  
     - MIP limits probetime
     - CPX_PARAM_PROBETIME
   * - :ref:`CPLEX_MIP_-_Probing_Time_Deterministic`  
     - MIP limits probedettime
     - CPX_PARAM_PROBEDETTIME
   * - :ref:`CPLEX_MIP_-_Rel_Difference_Obj`  
     - MIP tolerances relobjdifference
     - CPX_PARAM_RELOBJDIF
   * - :ref:`CPLEX_MIP_-_Select_Variables`  
     - MIP strategy variableselect
     - CPX_PARAM_VARSEL
   * - :ref:`CPLEX_MIP_-_Selection_of_Nodes`  
     - MIP strategy nodeselect
     - CPX_PARAM_NODESEL
   * - :ref:`CPLEX_MIP_-_Use_Generic_Callbacks` 
     - 
     - 
   * - :ref:`CPLEX_MIP_-_Working_Memory_Limit` 
     - Workmem
     - CPX_PARAM_WORKMEM
   * - :ref:`CPLEX_MIP_-_Write_MIP_Starts`  
     - 
     - 
   * - :ref:`CPLEX_MIP_Advanced_-_Find_Fractional_Root_Solution` 
     - 
     - 
   * - :ref:`CPLEX_MIP_Advanced_-_Lower_Objective_Stop`  
     - MIP limits lowerobjstop
     - CPX_PARAM_LOWEROBJSTOP
   * - :ref:`CPLEX_MIP_Advanced_-_SubMIP_Node_Limit` 
     - MIP submip nodelimit
     - CPX_PARAM_SUBMIPNODELIMIT
   * - :ref:`CPLEX_MIP_Advanced_-_SubMIP_Scale` 
     - MIP submip scale
     - CPX_PARAM_SUBMIPSCAIND
   * - :ref:`CPLEX_MIP_Advanced_-_SubMIP_Start_Algorithm` 
     - MIP submip startalg
     - CPX_PARAM_SUBMIPSTARTALG
   * - :ref:`CPLEX_MIP_Advanced_-_SubMIP_Subproblem_Algorithm` 
     - MIP submip subalg
     - CPX_PARAM_SUBMIPSUBALG
   * - :ref:`CPLEX_MIP_Advanced_-_Upper_Objective_Stop`  
     - MIP limits upperobjstop
     - CPX_PARAM_UPPEROBJSTOP
   * - :ref:`CPLEX_MIP_Advanced_-_Write_Cuts` 
     - 
     - 
   * - :ref:`CPLEX_MIP_Advanced_-_Write_Cuts_Variable_Val` 
     - 
     - 
   * - :ref:`CPLEX_Cuts_-_BQP_Cuts`  
     - MIP cuts bqp
     - CPX_PARAM_BQPCUTS
   * - :ref:`CPLEX_Cuts_-_Clique_Cuts`  
     - MIP cuts cliques
     - CPX_PARAM_CLIQUES
   * - :ref:`CPLEX_Cuts_-_Cover_Cuts` 
     - MIP cuts covers
     - CPX_PARAM_COVERS
   * - :ref:`CPLEX_Cuts_-_Cut_Gen_Limi` 
     - MIP limits aggforcut
     - CPX_PARAM_AGGCUTLIM
   * - :ref:`CPLEX_Cuts_-_Cut_Limit`  
     - MIP limits eachcutlimit
     - CPX_PARAM_EACHCUTLIM
   * - :ref:`CPLEX_Cuts_-_Cuts_Factor`  
     - MIP limits cutsfactor
     - CPX_PARAM_CUTSFACTOR
   * - :ref:`CPLEX_Cuts_-_Disjunct_Cuts` 
     - MIP cuts disjunctive
     - CPX_PARAM_DISJCUTS
   * - :ref:`CPLEX_Cuts_-_Flow_Cover_Cuts` 
     - MIP cuts flow
     - CPX_PARAM_FLOWCOVERS
   * - :ref:`CPLEX_Cuts_-_Flow_Path_Cuts` 
     - MIP cuts pathcut
     - CPX_PARAM_FLOWPATHS
   * - :ref:`CPLEX_Cuts_-_Gomory_Cuts` 
     - MIP cuts gomory
     - CPX_PARAM_FRACCUTS
   * - :ref:`CPLEX_Cuts_-_Gomory_Cuts_Cand` 
     - MIP limits gomorycand
     - CPX_PARAM_FRACCAND
   * - :ref:`CPLEX_Cuts_-_Gomory_Cuts_Pass_L` 
     - MIP limits gomorypass
     - CPX_PARAM_FRACPASS
   * - :ref:`CPLEX_Cuts_-_GUB_Cover_Cuts` 
     - MIP cuts gubcovers
     - CPX_PARAM_GUBCOVERS
   * - :ref:`CPLEX_Cuts_-_Implied_Bound_Cuts` 
     - MIP cuts implied
     - CPX_PARAM_IMPLBD
   * - :ref:`CPLEX_Cuts_-_Lift_and_Project_Cuts` 
     - MIP cuts liftproj
     - CPX_PARAM_LANDPCUTS
   * - :ref:`CPLEX_Cuts_-_Local_Implied_Bound_Cuts` 
     - MIP cuts localimplied
     - CPX_PARAM_LOCALIMPLBD
   * - :ref:`CPLEX_Cuts_-_MCF_Cuts`  
     - MIP cuts mcfcut
     - CPX_PARAM_MCFCUTS
   * - :ref:`CPLEX_Cuts_-_MIP_Nr_of_Cut_Pa` 
     - MIP limits cutpasses
     - CPX_PARAM_CUTPASS
   * - :ref:`CPLEX_Cuts_-_Mix_Integer_Round`  
     - MIP cuts mircut
     - CPX_PARAM_MIRCUTS
   * - :ref:`CPLEX_Cuts_-_Node_cuts`  
     - MIP cuts nodecuts
     - CPX_PARAM_NODECUTS
   * - :ref:`CPLEX_Cuts_-_RLT_Cuts`  
     - MIP cuts rlt
     - CPX_PARAM_RLTCUTS
   * - :ref:`CPLEX_Cuts_-_Zero_Half_Cuts`  
     - MIP cuts zerohalf
     - CPX_PARAM_ZEROHALFCUTS
   * - :ref:`CPLEX_MIP_Heuristic_-_Feasibility_Pump_Heuristic` 
     - MIP strategy fpheur
     - CPX_PARAM_FPHEUR
   * - :ref:`CPLEX_MIP_Heuristic_-_Heuristic_Effort` 
     - MIP strategy heuristiceffort
     - CPX_PARAM_HEUREFFORT
   * - :ref:`CPLEX_MIP_Heuristic_-_Heuristic_Freq` 
     - MIP strategy heuristicfreq
     - CPX_PARAM_HEURFREQ
   * - :ref:`CPLEX_MIP_Heuristic_-_Local_Branch_Heur` 
     - MIP strategy lbheur
     - CPX_PARAM_LBHEUR
   * - :ref:`CPLEX_MIP_Heuristic_-_RINS_Heurist_Freq` 
     - MIP strategy rinsheur
     - CPX_PARAM_RINSHEUR
   * - :ref:`CPLEX_MIP_Prepr_-_Boundstreng` 
     - Preprocessing boundstrength
     - CPX_PARAM_BNDSTRENIND
   * - :ref:`CPLEX_MIP_Prepr_-_Coef_Reduc` 
     - Preprocessing coeffreduce
     - CPX_PARAM_COEREDIND
   * - :ref:`CPLEX_MIP_Prepr_-_Preproc_Sym`  
     - Preprocessing symmetry
     - CPX_PARAM_SYMMETRY
   * - :ref:`CPLEX_MIP_Prepr_-_Presolve_Re`  
     - Preprocessing relax
     - CPX_PARAM_RELAXPREIND
   * - :ref:`CPLEX_MIP_Prepr_-_Repeat_Presolve`  
     - Preprocessing repeatpresolve
     - CPX_PARAM_REPEATPRESOLVE
   * - :ref:`CPLEX_MIP_Prepr_-_SOS1_Reformulations`  
     - Preprocessing sos1reform
     - CPX_PARAM_SOS1REFORM
   * - :ref:`CPLEX_MIP_Prepr_-_SOS2_Reformulations`  
     - Preprocessing sos2reform
     - CPX_PARAM_SOS2REFORM
   * - :ref:`CPLEX_Polishing_Absolute_MIP_Gap`  
     - MIP polishafter absmipgap
     - CPX_PARAM_POLISHAFTEREPAGAP
   * - :ref:`CPLEX_Polishing_Number_of_Nodes`  
     - MIP polishafter nodes
     - CPX_PARAM_POLISHAFTERNODE
   * - :ref:`CPLEX_Polishing_Number_of_Solutions`  
     - MIP polishafter solutions
     - CPX_PARAM_POLISHAFTERINTSOL
   * - :ref:`CPLEX_Polishing_Relative_MIP_Gap`  
     - MIP polishafter mipgap
     - CPX_PARAM_POLISHAFTEREPGAP
   * - :ref:`CPLEX_Polishing_Time`  
     - MIP polishafter time
     - CPX_PARAM_POLISHAFTERTIME
   * - :ref:`CPLEX_Polishing_Time_Deterministic`  
     - MIP polishafter dettime
     - CPX_PARAM_POLISHAFTERDETTIME
   * - :ref:`CPLEX_MIP_Solp_-_Do_Populate`  
     - 
     - 
   * - :ref:`CPLEX_MIP_Solp_-_Pool_Abs_Obj_Gap` 
     - MIP pool absgap
     - CPX_PARAM_SOLNPOOLAGAP
   * - :ref:`CPLEX_MIP_Solp_-_Pool_Capacity`  
     - MIP pool capacity
     - CPX_PARAM_SOLNPOOLCAPACITY
   * - :ref:`CPLEX_MIP_Solp_-_Pool_Intensity`  
     - MIP pool intensity
     - CPX_PARAM_SOLNPOOLINTENSITY
   * - :ref:`CPLEX_MIP_Solp_-_Pool_Rel_Obj_Gap` 
     - MIP pool relgap
     - CPX_PARAM_SOLNPOOLGAP
   * - :ref:`CPLEX_MIP_Solp_-_Pool_Repl_Strat`  
     - MIP pool replace
     - CPX_PARAM_SOLNPOOLREPLACE
   * - :ref:`CPLEX_MIP_Solp_-_Populate_time_limit`  
     - 
     - 
   * - :ref:`CPLEX_MIP_Solp_-_Population_Limit`  
     - MIP limits populate
     - CPX_PARAM_POPULATELIM
   * - :ref:`CPLEX_-_Network_Extraction_L` 
     - Network netfind
     - CPX_PARAM_NETFIND
   * - :ref:`CPLEX_-_Network_Feasibility` 
     - Network tolerances feasibility
     - CPX_PARAM_NETEPRHS
   * - :ref:`CPLEX_-_Network_Iterations` 
     - Network iterations
     - CPX_PARAM_NETITLIM
   * - :ref:`CPLEX_-_Network_Optimality` 
     - Network tolerances optimality
     - CPX_PARAM_NETEPOPT
   * - :ref:`CPLEX_-_Network_Pricing` 
     - Network pricing
     - CPX_PARAM_NETPPRIIND
   * - :ref:`CPLEX_Par_-_Auxiliary_Root_Threads` 
     - MIP limits auxrootthreads
     - CPX_PARAM_AUXROOTTHREADS
   * - :ref:`CPLEX_Par_-_GlobalThreadLimit` 
     - Threads
     - CPX_PARAM_THREADS
   * - :ref:`CPLEX_Par_-_Parallel_Mode` 
     - Parallel mode
     - CPX_PARAM_PARALLELMODE
   * - :ref:`CPLEX_Prepr_-_Aggregator` 
     - Preprocessing aggregator
     - CPX_PARAM_AGGIND
   * - :ref:`CPLEX_Prepr_-_Dependency` 
     - Preprocessing dependency
     - CPX_PARAM_DEPIND
   * - :ref:`CPLEX_Prepr_-_Folding` 
     - Preprocessing folding
     - CPX_PARAM_FOLDING
   * - :ref:`CPLEX_Prepr_-_Limit_Substitut`  
     - Preprocessing fill
     - CPX_PARAM_AGGFILL
   * - :ref:`CPLEX_Prepr_-_Number_of_IterP` 
     - Preprocessing numpass
     - CPX_PARAM_PREPASS
   * - :ref:`CPLEX_Prepr_-_Pre_reduction_types`  
     - Preprocessing reduce
     - CPX_PARAM_REDUCE
   * - :ref:`CPLEX_Prepr_-_Presolve`  
     - Preprocessing presolve
     - CPX_PARAM_PREIND
   * - :ref:`CPLEX_Prepr_-_Presolve_Pass_D` 
     - Preprocessing dual
     - CPX_PARAM_PREDUAL
   * - :ref:`CPLEX_Prepr_-_Print_Prslv_Sta`  
     - 
     - 
   * - :ref:`CPLEX_QP_-_Adjust_MIQP`  
     - Preprocessing qpmakepsd
     - CPX_PARAM_QPMAKEPSDIND
   * - :ref:`CPLEX_QP_-_Barrier_Conv_Toler`  
     - Bar qcpconvergetol
     - CPX_PARAM_BARQCPEPCOMP
   * - :ref:`CPLEX_QP_-_MIQCP_Strategy`  
     - MIP strategy miqcpstrat
     - CPX_PARAM_MIQCPSTRAT
   * - :ref:`CPLEX_QP_-_QCP_Dual_Values`  
     - Preprocessing qcpduals
     - CPX_PARAM_CALCQCPDUALS
   * - :ref:`CPLEX_QP_-_QP_Linearization`  
     - Preprocessing qtolin
     - CPX_PARAM_QTOLININD
   * - :ref:`CPLEX_QP_-_QP_Method`  
     - Qpmethod
     - CPX_PARAM_QPMETHOD
   * - :ref:`CPLEX_QP_-_QP_Nonzeros_Read_Limit`  
     - Read qpnonzeros
     - CPX_PARAM_QPNZREADLIM
   * - :ref:`CPLEX_QP_-_Solution_Target`  
     - Optimalitytarget
     - CPX_PARAM_OPTIMALITYTARGET
   * - :ref:`CPLEX_Simplex_-_Crash_Ordering`  
     - Simplex crash
     - CPX_PARAM_CRAIND
   * - :ref:`CPLEX_Simplex_-_Dual_Pric_Alg`  
     - Simplex dgradient
     - CPX_PARAM_DPRIIND
   * - :ref:`CPLEX_Simplex_-_Dynamic_Row_Management`  
     - simplex dynamicrows
     - CPX_PARAM_DYNAMICROWS
   * - :ref:`CPLEX_Simplex_-_Feasibility`  
     - Simplex tolerances feasibility
     - CPX_PARAM_EPRHS
   * - :ref:`CPLEX_Simplex_-_Markowitz` 
     - Simplex tolerances markowitz
     - CPX_PARAM_EPMRK
   * - :ref:`CPLEX_Simplex_-_Optimality`  
     - Simplex tolerances optimality
     - CPX_PARAM_EPOPT
   * - :ref:`CPLEX_Simplex_-_Perturb_Const`  
     - Simplex perturbationlimit
     - CPX_PARAM_EPPER
   * - :ref:`CPLEX_Simplex_-_Perturb_Indic` 
     - Simplex perturbationlimit
     - CPX_PARAM_PERIND
   * - :ref:`CPLEX_Simplex_-_Pricing`  
     - Simplex pricing
     - CPX_PARAM_PRICELIM
   * - :ref:`CPLEX_Simplex_-_Prim_Pric_Alg`  
     - Simplex pgradient
     - CPX_PARAM_PPRIIND
   * - :ref:`CPLEX_Simplex_-_Refactor`  
     - Simplex refactor
     - CPX_PARAM_REINV
   * - :ref:`CPLEX_Simplex_-_Sifting_from_Simplex` 
     - Sifting simplex
     - CPX_PARAM_SIFTSIM
   * - :ref:`CPLEX_Simplex_-_Singular` 
     - Simplex limits singularity
     - CPX_PARAM_SINGLIM
   * - :ref:`CPLEX_Simplex_-_Stalled_Iter`  
     - Simplex limits perturbation
     - CPX_PARAM_PERLIM
   * - :ref:`CPLEX_Tuning_-_Tuning_Measure` 
     - Tune measure
     - CPX_PARAM_TUNINGMEASURE
   * - :ref:`CPLEX_Tuning_-_Tuning_Repeater` 
     - Tune repeat
     - CPX_PARAM_TUNINGREPEAT
   * - :ref:`CPLEX_Tuning_-_Tuning_Time_Limit` 
     - Tune timelimit
     - CPX_PARAM_TUNINGTILIM
   * - :ref:`CPLEX_Tuning_-_Tuning_Time_Limit_Deter` 
     - Tune dettimelimit
     - CPX_PARAM_TUNINGDETTILIM






The table below shows Solvers General options that are mapped to CPLEX 22.1 parameters.




.. list-table::

   * - **Option name in AIMMS** 
     - **Name in CPLEX** 
     - **Name in CPLEX C API** 
   * - :ref:`Options_MIP_Options_-_Cutoff` 
     - MIP tolerances lowercutoff
     - CPX_PARAM_CUTLO
   * - 
     - MIP tolerances uppercutoff
     - CPX_PARAM_CUTUP
   * - :ref:`Options_MIP_Options_-_Maximal_Number_o` 
     - MIP limits solutions
     - CPX_PARAM_INTSOLLIM
   * - :ref:`Options_MIP_Options_-_MIP_Absolute_Opt` 
     - MIP tolerances absmipgap
     - CPX_PARAM_EPAGAP
   * - :ref:`Options_MIP_Options_-_MIP_Relative_Opt` 
     - MIP tolerances mipgap
     - CPX_PARAM_EPGAP
   * - :ref:`Options_Stop_Criteria_-_Iteration_Limi` 
     - Simplex limits iterations
     - CPX_PARAM_ITLIM
   * - :ref:`Options_Stop_Criteria_-_Time_Limit` 
     - Timelimit
     - CPX_PARAM_TILIM


