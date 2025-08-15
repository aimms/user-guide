

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
     - :ref:`ODH-CPLEX_General_-_Qui


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


**Heuristic sub-model parameters** 

The heuristic sub-model parameters can only be set using a :ref:`ODH-CPLEX_-_Parameter_File` . The syntax for the parameters that influence the heuristic sub-model CPLEX solves is the following: SUB_<parameter> where <parameter> refers to the ODH-CPLEX name in the second table above. The syntax for the parameters that influence the heuristic sub-model CPLEX solves in Phase I is the following: PHASE1_<parameter>.



For example, SUB_CPX_RINSHEUR specifies the RINS heuristic frequency for CPLEX if it used to solve a heuristic sub-model, while PHASE1_CPX_RINSHEUR specifies the RINS heuristic frequency for CPLEX if it used to solve a heuristic sub-model in Phase I.



**Learn more about** 

*	:ref:`ODH-CPLEX_-_Parameter_File` 
*	:ref:`ODH-CPLEX_General_-_Search_Mode`  
