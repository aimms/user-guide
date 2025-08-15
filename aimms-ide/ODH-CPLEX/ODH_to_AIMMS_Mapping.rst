

.. _ODH_to_AIMMS_Mapping:
.. _ODH-CPLEX_ODH_to_AIMMS_Mapping:


ODH to AIMMS Mapping
========================

**ODH engine parameters** 

The table below shows in the left column the ODH engine parameters from ODH-CPLEX that can be set in AIMMS; the right column displays for each ODH-CPLEX 5.3 parameter the associated AIMMS option.

.. list-table::

   * - **Name in ODH-CPLEX**
     - **Option name in AIMMS**
   * - DECOMPDENSITY
     - :ref:`ODH-CPLEX_Advanced_-_Decomposition_Density`
   * - DETERMINISTIC
     - :ref:`ODH-CPLEX_Heuristic_-_Sol_Impr_Heur_Mode`
   * - DIVISOR
     - :ref:`ODH-CPLEX_Advanced_-_Initial_Divisor_Value_Sub`
   * - FEASOPT
     - :ref:`ODH-CPLEX_Advanced_-_Optimization_Method`
   * - FEASTOL
     - :ref:`ODH-CPLEX_General_-_ODH_Feasibility_Tolerance`
   * - FIRSTFEAS
     - :ref:`ODH-CPLEX_Heuristic_-_First_Feasible_Heuristic`
   * - FIRSTFEASCONTINUE
     - :ref:`ODH-CPLEX_Heuristic_-_First_Feasible_Heuristic_Continue`
   * - FIRSTFEASEFFORT
     - :ref:`ODH-CPLEX_Heuristic_-_First_Feasible_Heuristic_Effort_Level`
   * - FIRSTFEASSHIFT
     - :ref:`ODH-CPLEX_Heuristic_-_First_Feasible_Heuristic_Shift`
   * - GLOBALBOUNDS
     - :ref:`ODH-CPLEX_Advanced_-_Global_Bounds`
   * - INTERDIV
     - :ref:`ODH-CPLEX_Advanced_-_Initial_Divisor_Value`
   * - MAXBACKTRACK
     - :ref:`ODH-CPLEX_Advanced_-_Backtrack_Limit`
   * - MAXINFREPEAT
     - :ref:`ODH-CPLEX_Advanced_-_Maximum_Divisor_Repeats_Inf`
   * - MAXINTERDIV
     - :ref:`ODH-CPLEX_Advanced_-_Maximum_Divisor_Value`
   * - MAXREPEAT
     - :ref:`ODH-CPLEX_Advanced_-_Maximum_Divisor_Repeats`
   * - OBJTARGET
     - :ref:`ODH-CPLEX_General_-_Objective_Target`
   * - ODHPRESOLVE
     - :ref:`ODH-CPLEX_General_-_ODH_Presolve`
   * - PENALTY
     - :ref:`ODH-CPLEX_Heuristic_-_Sol_Impr_Heur_Penalty`
   * - PHASE12
     - :ref:`ODH-CPLEX_General_-_Remove_Inf_Method`
   * - PRESOLVE
     - :ref:`ODH-CPLEX_General_-_Presolve`
   * - PROCESSORLOCK
     - :ref:`ODH-CPLEX_Parallel_-_Processor_Lock`
   * - QUICKFIRSTSOLVE
     - :ref:`ODH-CPLEX_General_-_Quick_First_Solve`
   * - RECURSE
     - :ref:`ODH-CPLEX_Heuristic_-_Recurse`
   * - RECURSEDECOMP
     - :ref:`ODH-CPLEX_Heuristic_-_Recurse_Decomposition_Method`
   * - RECURSEITERLIM
     - :ref:`ODH-CPLEX_Heuristic_-_Recurse_Iteration_Limit`
   * - RECURSELOG
     - :ref:`ODH-CPLEX_Logging_-_Recurse_Log`
   * - RECURSEMINITERLIM
     - :ref:`ODH-CPLEX_Heuristic_-_Recurse_Minimum_Iterations`
   * - RECURSESOLITERLIM
     - :ref:`ODH-CPLEX_Heuristic_-_Recurse_Iteration_Limit_Solution`
   * - REJECTINFSOL
     - :ref:`ODH-CPLEX_General_-_Reject_Inf_Solutions`
   * - RELAXSOS2
     - :ref:`ODH-CPLEX_General_-_Relax_SOS2`
   * - SEED
     - :ref:`ODH-CPLEX_General_-_ODH_Seed`
   * - STRATEGY
     - :ref:`ODH-CPLEX_Heuristic_-_Sol_Impr_Heur_Strategy`
   * - SYNCFREQ
     - :ref:`ODH-CPLEX_Parallel_-_Thread_Sync_Freq`
   * - THREADLOG
     - :ref:`ODH-CPLEX_Logging_-_Thread_Log`
   * - THREADS
     - :ref:`ODH-CPLEX_Parallel_-_Thread_Limit`
   * - TIMELIMIT
     - :ref:`Options_Stop_Criteria_-_Time_Limit`
   * - VARIABLECLEAN
     - :ref:`ODH-CPLEX_General_-_Clean_variables_sub_models`
   * - WRITESOLUTION
     - :ref:`ODH-CPLEX_General_-_Write_Solution_File`


**Main CPLEX solve parameters** 

The table below shows CPLEX options for the main CPLEX solve in ODH-CPLEX (if the **Search Mode**  is set to 'Global Solution') or for getting an initial feasible solution (if the **Search Mode**  is set to 'Local Solution'). 
The table below shows in the left column the CPLEX parameters from ODH-CPLEX that can be set in AIMMS; the right column displays for each ODH-CPLEX 5.3 parameter the associated AIMMS option.

.. list-table::

   * - **Name in ODH-CPLEX**
     - **Option name in AIMMS**
   * - CPX_ADVIND
     - :ref:`ODH-CPLEX_XGeneral_-_AdvancedStart`
   * - CPX_AGGCUTLIM
     - :ref:`ODH-CPLEX_XCuts_-_Cut_Gen_Limi`
   * - CPX_AGGFILL
     - :ref:`ODH-CPLEX_XPrepr_-_Limit_Substitut`
   * - CPX_AGGIND
     - :ref:`ODH-CPLEX_XPrepr_-_Aggregator`
   * - CPX_AUXROOTTHREADS
     - :ref:`ODH-CPLEX_XPar_-_Auxiliary_Root_Threads`
   * - CPX_BARALG
     - :ref:`ODH-CPLEX_XBarrier_-_Barrier_Algorithm`
   * - CPX_BARCOLNZ
     - :ref:`ODH-CPLEX_XBarrier_-_Barrier_Density_Defi`
   * - CPX_BARCROSSALG
     - :ref:`ODH-CPLEX_XBarrier_-_Barrier_cross`
   * - CPX_BARDISPLAY
     - :ref:`ODH-CPLEX_XLogging_-_Barrier_Display`
   * - CPX_BAREPCOMP
     - :ref:`ODH-CPLEX_XBarrier_-_Barrier_Convergence_`
   * - CPX_BARGROWTH
     - :ref:`ODH-CPLEX_XBarrier_-_Barrier_Growth_Limit`
   * - CPX_BARITLIM
     - :ref:`ODH-CPLEX_XBarrier_-_Barrier_Iterations`
   * - CPX_BARMAXCOR
     - :ref:`ODH-CPLEX_XBarrier_-_Barrier_Maximal_Numb`
   * - CPX_BAROBJRNG
     - :ref:`ODH-CPLEX_XBarrier_-_Barrier_Objective_Ra`
   * - CPX_BARORDER
     - :ref:`ODH-CPLEX_XBarrier_-_Barrier_Ordering`
   * - CPX_BARQCPEPCOMP
     - :ref:`ODH-CPLEX_XQuadratic_-_Barrier_Conv_Toler`
   * - CPX_BARSTARTALG
     - :ref:`ODH-CPLEX_XBarrier_-_Barrier_Start_Algori`
   * - CPX_BNDSTRENIND
     - :ref:`ODH-CPLEX_XMIP_Prepr_-_Boundstreng`
   * - CPX_BQPCUTS
     - :ref:`ODH-CPLEX_XCuts_-_BQP_Cuts`
   * - CPX_BRDIR
     - :ref:`ODH-CPLEX_XMIP_-_Branch`
   * - CPX_BTTOL
     - :ref:`ODH-CPLEX_XMIP_-_Backtrack`
   * - CPX_CLIQUES
     - :ref:`ODH-CPLEX_XCuts_-_Clique_Cuts`
   * - CPX_CLOCKTYPE
     - :ref:`ODH-CPLEX_XGeneral_-_Clock_Type`
   * - CPX_CLONELOG
     - :ref:`ODH-CPLEX_XLogging_-_Clone_Log_Files`
   * - CPX_COEREDIND
     - :ref:`ODH-CPLEX_XMIP_Prepr_-_Coef_Reduc`
   * - CPX_CONFLICTALG
     - :ref:`ODH-CPLEX_XGeneral_-_Conflict_Algorithm`
   * - CPX_COVERS
     - :ref:`ODH-CPLEX_XCuts_-_Cover_Cuts`
   * - CPX_CRAIND
     - :ref:`ODH-CPLEX_XSimplex_-_Crash_Ordering`
   * - CPX_CUTLO
     - :ref:`Options_MIP_Options_-_Cutoff`
   * - CPX_CUTPASS
     - :ref:`ODH-CPLEX_XCuts_-_MIP_Nr_of_Cut_Pa`
   * - CPX_CUTSFACTOR
     - :ref:`ODH-CPLEX_XCuts_-_Cuts_Factor`
   * - CPX_CUTUP
     - :ref:`Options_MIP_Options_-_Cutoff`
   * - CPX_DATACHECK
     - :ref:`ODH-CPLEX_XGeneral_-_Data_Check`
   * - CPX_DEPIND
     - :ref:`ODH-CPLEX_XPrepr_-_Dependency`
   * - CPX_DETTILIM
     - :ref:`ODH-CPLEX_XGeneral_-_Deterministic_Time_Limit`
   * - CPX_DISJCUTS
     - :ref:`ODH-CPLEX_XCuts_-_Disjunct_Cuts`
   * - CPX_DIVETYPE
     - :ref:`ODH-CPLEX_XMIP_-_MIP_Dive_Strat`
   * - CPX_DPRIIND
     - :ref:`ODH-CPLEX_XSimplex_-_Dual_Pric_Alg`
   * - CPX_DYNAMICROWS
     - :ref:`ODH-CPLEX_XSimplex_-_Dynamic_Row_Management`
   * - CPX_EACHCUTLIM
     - :ref:`ODH-CPLEX_XCuts_-_Cut_Limit`
   * - CPX_EPAGAP
     - :ref:`Options_MIP_Options_-_MIP_Absolute_Opt`
   * - CPX_EPGAP
     - :ref:`Options_MIP_Options_-_MIP_Relative_Opt`
   * - CPX_EPINT
     - :ref:`ODH-CPLEX_XMIP_-_Integrality`
   * - CPX_EPMRK
     - :ref:`ODH-CPLEX_XSimplex_-_Markowitz`
   * - CPX_EPOPT
     - :ref:`ODH-CPLEX_XSimplex_-_Optimality`
   * - CPX_EPPER
     - :ref:`ODH-CPLEX_XSimplex_-_Perturb_Const`
   * - CPX_EPRHS
     - :ref:`ODH-CPLEX_XSimplex_-_Feasibility`
   * - CPX_FLOWCOVERS
     - :ref:`ODH-CPLEX_XCuts_-_Flow_Cover_Cuts`
   * - CPX_FLOWPATHS
     - :ref:`ODH-CPLEX_XCuts_-_Flow_Path_Cuts`
   * - CPX_FOLDING
     - :ref:`ODH-CPLEX_XPrepr_-_Folding`
   * - CPX_FPHEUR
     - :ref:`ODH-CPLEX_XMIP_Heuristic_-_Feasibility_Pump_Heuristic`
   * - CPX_FRACCAND
     - :ref:`ODH-CPLEX_XCuts_-_Gomory_Cuts_Cand`
   * - CPX_FRACCUTS
     - :ref:`ODH-CPLEX_XCuts_-_Gomory_Cuts`
   * - CPX_FRACPASS
     - :ref:`ODH-CPLEX_XCuts_-_Gomory_Cuts_Pass_L`
   * - CPX_GUBCOVERS
     - :ref:`ODH-CPLEX_XCuts_-_GUB_Cover_Cuts`
   * - CPX_HEUREFFORT
     - :ref:`ODH-CPLEX_XMIP_Heuristic_-_Heuristic_Effort`
   * - CPX_HEURFREQ
     - :ref:`ODH-CPLEX_XMIP_Heuristic_-_Heuristic_Freq`
   * - CPX_IMPLBD
     - :ref:`ODH-CPLEX_XCuts_-_Implied_Bound_Cuts`
   * - CPX_INTSOLLIM
     - :ref:`Options_MIP_Options_-_Maximal_Number_o`
   * - CPX_ITLIM
     - :ref:`Options_Stop_Criteria_-_Iteration_Limi`
   * - CPX_LANDPCUTS
     - :ref:`ODH-CPLEX_XCuts_-_Lift_and_Project_Cuts`
   * - CPX_LBHEUR
     - :ref:`ODH-CPLEX_XMIP_Heuristic_-_Local_Branch_Heur`
   * - CPX_LOCALIMPLBD
     - :ref:`ODH-CPLEX_XCuts_-_Local_Implied_Bound_Cuts`
   * - CPX_MCFCUTS
     - :ref:`ODH-CPLEX_XCuts_-_MCF_Cuts`
   * - CPX_MEMORYEMPHASIS
     - :ref:`ODH-CPLEX_XGeneral_-_MemoryEmphasis`
   * - CPX_MIPDISPLAY
     - :ref:`ODH-CPLEX_XLogging_-_MIP_Display`
   * - CPX_MIPEMPHASIS
     - :ref:`ODH-CPLEX_XMIP_-_MIP_Emphasis`
   * - CPX_MIPINTERVAL
     - :ref:`ODH-CPLEX_XLogging_-_MIP_Interval`
   * - CPX_MIPORDIND
     - :ref:`ODH-CPLEX_XMIP_-_MIP_Priority_Order_Switch`
   * - CPX_MIPORDTYPE
     - :ref:`ODH-CPLEX_XMIP_-_MIP_Priority_Order_Type`
   * - CPX_MIPSEARCH
     - :ref:`ODH-CPLEX_XMIP_-_MIP_Search_Strategy`
   * - CPX_MIQCPSTRAT
     - :ref:`ODH-CPLEX_XQuadratic_-_MIQCP_Strategy`
   * - CPX_MIRCUTS
     - :ref:`ODH-CPLEX_XCuts_-_Mix_Integer_Round`
   * - CPX_NETEPOPT
     - :ref:`ODH-CPLEX_XNetwork_-_Network_Optimality`
   * - CPX_NETEPRHS
     - :ref:`ODH-CPLEX_XNetwork_-_Network_Feasibility`
   * - CPX_NETITLIM
     - :ref:`ODH-CPLEX_XNetwork_-_Network_Iterations`
   * - CPX_NETPPRIIND
     - :ref:`ODH-CPLEX_XNetwork_-_Network_Pricing`
   * - CPX_NODECUTS
     - :ref:`ODH-CPLEX_XCuts_-_Node_Cuts`
   * - CPX_NODEFILEIND
     - :ref:`ODH-CPLEX_XMIP_-_Node_File`
   * - CPX_NODELIM
     - :ref:`ODH-CPLEX_XMIP_-_Max_Nr_of_Nodes`
   * - CPX_NODESEL
     - :ref:`ODH-CPLEX_XMIP_-_Selection_of_Nodes`
   * - CPX_NUMERICALEMPHASIS
     - :ref:`ODH-CPLEX_XGeneral_-_NumericalEmphasis`
   * - CPX_OBJDIF
     - :ref:`ODH-CPLEX_XMIP_-_Difference_Object`
   * - CPX_OPTIMALITYTARGET
     - :ref:`ODH-CPLEX_XQuadratic_-_Solution_Target`
   * - CPX_PARALLELMODE
     - :ref:`ODH-CPLEX_XPar_-_Parallel_Mode`
   * - CPX_PERIND
     - :ref:`ODH-CPLEX_XSimplex_-_Perturb_Indic`
   * - CPX_PERLIM
     - :ref:`ODH-CPLEX_XSimplex_-_Stalled_Iter`
   * - CPX_POLISHAFTERDETTIME
     - :ref:`ODH-CPLEX_XPolishing_Time_Deterministic`
   * - CPX_POLISHAFTEREPAGAP
     - :ref:`ODH-CPLEX_XPolishing_Absolute_MIP_Gap`
   * - CPX_POLISHAFTEREPGAP
     - :ref:`ODH-CPLEX_XPolishing_Relative_MIP_Gap`
   * - CPX_POLISHAFTERINTSOL
     - :ref:`ODH-CPLEX_XPolishing_Number_of_Solutions`
   * - CPX_POLISHAFTERNODE
     - :ref:`ODH-CPLEX_XPolishing_Number_of_Nodes`
   * - CPX_POLISHAFTERTIME
     - :ref:`ODH-CPLEX_XPolishing_Time`
   * - CPX_POPULATELIM
     - :ref:`ODH-CPLEX_XMIP_Solp_-_Population_Limit`
   * - CPX_PREDUAL
     - :ref:`ODH-CPLEX_XPrepr_-_Presolve_Pass_D`
   * - CPX_PREPASS
     - :ref:`ODH-CPLEX_XPrepr_-_Number_of_IterP`
   * - CPX_PRESLVND
     - :ref:`ODH-CPLEX_XMIP_-_MIP_Node_Presolve`
   * - CPX_PRICELIM
     - :ref:`ODH-CPLEX_XSimplex_-_Pricing`
   * - CPX_PROBE
     - :ref:`ODH-CPLEX_XMIP_-_MIP_Probing`
   * - CPX_PROBEDETTIME
     - :ref:`ODH-CPLEX_XMIP_-_Probing_Time_Deterministic`
   * - CPX_PROBETIME
     - :ref:`ODH-CPLEX_XMIP_-_Probing_Time`
   * - CPX_PPRIIND
     - :ref:`ODH-CPLEX_XSimplex_-_Prim_Pric_Alg`
   * - CPX_QPMAKEPSDIND
     - :ref:`ODH-CPLEX_XQuadratic_-_Adjust_MIQP`
   * - CPX_QPMETHOD
     - :ref:`ODH-CPLEX_XQuadratic_-_QP_Method`
   * - CPX_QPNZREADLIM
     - :ref:`ODH-CPLEX_XQuadratic_-_QP_Nonzeros_Read_Limit`
   * - CPX_QTOLININD
     - :ref:`ODH-CPLEX_XQuadratic_-_QP_Linearization`
   * - CPX_RANDOMSEED
     - :ref:`ODH-CPLEX_XGeneral_-_Random_Seed`
   * - CPX_REDUCE
     - :ref:`ODH-CPLEX_XPrepr_-_Pre_reduction_types`
   * - CPX_REINV
     - :ref:`ODH-CPLEX_XSimplex_-_Refactor`
   * - CPX_RELAXPREIND
     - :ref:`ODH-CPLEX_XMIP_Prepr_-_Presolve_Re`
   * - CPX_RELOBJDIF
     - :ref:`ODH-CPLEX_XMIP_-_Rel_Difference_Obj`
   * - CPX_REPAIRTRIES
     - :ref:`ODH-CPLEX_XMIP_-_NumberofRepairAttempts`
   * - CPX_REPEATPRESOLVE
     - :ref:`ODH-CPLEX_XMIP_Prepr_-_Repeat_Presolve`
   * - CPX_RINSHEUR
     - :ref:`ODH-CPLEX_XMIP_Heuristic_-_RINS_Heurist_Freq`
   * - CPX_RLTCUTS
     - :ref:`ODH-CPLEX_XCuts_-_RLT_Cuts`
   * - CPX_SCAIND
     - :ref:`ODH-CPLEX_XGeneral_-_Scale`
   * - CPX_SIFTALG
     - :ref:`ODH-CPLEX_XGeneral_-_Sifting_Algorithm`
   * - CPX_SIFTSIM
     - :ref:`ODH-CPLEX_XSimplex_-_Sifting_from_Simplex`
   * - CPX_SIMDISPLAY
     - :ref:`ODH-CPLEX_XLogging_-_Simplex_Display`
   * - CPX_SINGLIM
     - :ref:`ODH-CPLEX_XSimplex_-_Singular`
   * - CPX_SOLNPOOLAGAP
     - :ref:`ODH-CPLEX_XMIP_Solp_-_Pool_Abs_Obj_Gap`
   * - CPX_SOLNPOOLCAPACITY
     - :ref:`ODH-CPLEX_XMIP_Solp_-_Pool_Capacity`
   * - CPX_SOLNPOOLGAP
     - :ref:`ODH-CPLEX_XMIP_Solp_-_Pool_Rel_Obj_Gap`
   * - CPX_SOLNPOOLINTENSITY
     - :ref:`ODH-CPLEX_XMIP_Solp_-_Pool_Intensity`
   * - CPX_SOLNPOOLREPLACE
     - :ref:`ODH-CPLEX_XMIP_Solp_-_Pool_Repl_Strat`
   * - CPX_SOS1REFORM
     - :ref:`ODH-CPLEX_XMIP_Prepr_-_SOS1_Reformulations`
   * - CPX_SOS2REFORM
     - :ref:`ODH-CPLEX_XMIP_Prepr_-_SOS2_Reformulations`
   * - CPX_STARTALG
     - :ref:`ODH-CPLEX_XMIP_-_MIP_Start_Algorit`
   * - CPX_STRONGCANDLIM
     - :ref:`ODH-CPLEX_XMIP_-_MIP_Cand_List`
   * - CPX_STRONGITLIM
     - :ref:`ODH-CPLEX_XMIP_-_Nr_of_Simplex_Iter`
   * - CPX_SUBALG
     - :ref:`ODH-CPLEX_XMIP_-_MIP_Method`
   * - CPX_SUBMIPNODELIMIT
     - :ref:`ODH-CPLEX_XMIP_Advanced_-_SubMIP_Node_Limit`
   * - CPX_SUBMIPSCAIND
     - :ref:`ODH-CPLEX_XMIP_Advanced_-_SubMIP_Scale`
   * - CPX_SUBMIPSTARTALG
     - :ref:`ODH-CPLEX_XMIP_Advanced_-_SubMIP_Start_Algorithm`
   * - CPX_SUBMIPSUBALG
     - :ref:`ODH-CPLEX_XMIP_Advanced_-_SubMIP_Subproblem_Algorithm`
   * - CPX_SYMMETRY
     - :ref:`ODH-CPLEX_XMIP_Prepr_-_Preproc_Sym`
   * - CPX_THREADS
     - :ref:`ODH-CPLEX_XPar_-_GlobalThreadLimit`
   * - CPX_TRELIM
     - :ref:`ODH-CPLEX_XMIP_-_MIP_Tree_Memory_Limit`
   * - CPX_VARSEL
     - :ref:`ODH-CPLEX_XMIP_-_Select_Variables`
   * - CPX_WORKMEM
     - :ref:`ODH-CPLEX_XMIP_-_Working_Memory_Limit`
   * - CPX_ZEROHALFCUTS
     - :ref:`ODH-CPLEX_XCuts_-_Zero_Half_Cuts`


**Heuristic sub-model parameters** 

The heuristic sub-model parameters can only be set using a :ref:`ODH-CPLEX_-_Parameter_File` . The syntax for the parameters that influence the heuristic sub-model CPLEX solves is the following: SUB_<parameter> where <parameter> refers to the ODH-CPLEX name in the second table above. The syntax for the parameters that influence the heuristic sub-model CPLEX solves in Phase I is the following: PHASE1_<parameter>.



For example, SUB_CPX_RINSHEUR specifies the RINS heuristic frequency for CPLEX if it used to solve a heuristic sub-model, while PHASE1_CPX_RINSHEUR specifies the RINS heuristic frequency for CPLEX if it used to solve a heuristic sub-model in Phase I.



**Learn more about** 

*	:ref:`ODH-CPLEX_-_Parameter_File` 
*	:ref:`ODH-CPLEX_General_-_Search_Mode`  
