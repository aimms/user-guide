

.. _CBC_to_AIMMS_Mapping:


CBC to AIMMS Mapping
====================

**Description** 

The table shows in the left column the parameters from CBC that can be set in AIMMS; the right column displays for each CBC parameter the associated AIMMS option.



.. list-table::

   * - **Name in CBC**
     - **Option name in AIMMS**
   * - bscale
     - :doc:`Barrier - Barrier scaling <Barrier/CBC_Barrier_-_Barrier_Scaling>`
   * - cliqueCuts
     - :doc:`MIP Cuts - Clique cuts <MIP Cuts/CBC_MIP_Cuts_-_Clique_Cuts>`
   * - combineSolutions
     - :doc:`MIP Heuristics - Combine solutions <MIP Heuristics/CBC_MIP_Heur_-_Combine_solutions>`
   * - costStrategy
     - :doc:`MIP - Variable selection <MIP/CBC_MIP_-_Variable_Selection>`
   * - crash
     - :doc:`Simplex - Crash <Simplex/CBC_Simplex_-_Crash>`
   * - crossover
     - :doc:`Barrier - Barrier crossover <Barrier/CBC_Barrier_-_Barrier_crossover>`
   * - cutDepth
     - :doc:`MIP Cuts - Cut depth <MIP Cuts/CBC_MIP_Cuts_-_Cut_Depth>`
   * - cuts
     - :doc:`MIP Cuts - Global cut control <MIP Cuts/CBC_MIP_Cuts_-_Global_Cut_Control>`
   * - dualTolerance
     - :doc:`General - Dual feasibility tolerance <General/CBC_General_-_Dual_Feasibility_Tol>`
   * - dualPivot
     - :doc:`Simplex - Dual pivot <Simplex/CBC_Simplex_-_Dual_pivot>`
   * - feasibilityPump
     - :doc:`MIP Heuristics - Feasibility pump <MIP Heuristics/CBC_MIP_Heur_-_Feasibility_pump>`
   * - flowCoverCuts
     - :doc:`MIP Cuts - Flow cover cuts <MIP Cuts/CBC_MIP_Cuts_-_Flow_Cover_Cuts>`
   * - gomoryCuts
     - :doc:`MIP Cuts - Gomory cuts <MIP Cuts/CBC_MIP_Cuts_-_Gomory_Cuts>`
   * - greedyHeuristic
     - :doc:`MIP Heuristics - Greedy heuristic <MIP Heuristics/CBC_MIP_Heur_-_Greedy_heuristic>`
   * - heuristicsOnOff
     - :doc:`MIP Heuristics - Heuristics <MIP Heuristics/CBC_MIP_Heur_-_Heuristics>`
   * - idiotCrash
     - :doc:`Simplex - Idiot crash <Simplex/CBC_Simplex_-_Idiot_crash>`
   * - increment
     - :doc:`MIP - Increment <MIP/CBC_MIP_-_Increment>`
   * - integerTolerance
     - :doc:`MIP - Integrality <MIP/CBC_MIP_-_Integrality>`
   * - knapsackCuts
     - :doc:`MIP Cuts - Knapsack cuts <MIP Cuts/CBC_MIP_Cuts_-_Knapsack_Cuts>`
   * - liftAndProjectCuts
     - :doc:`MIP Cuts - Lift and project cuts <MIP Cuts/CBC_MIP_Cuts_-_Lift_and_Project_Cuts>`
   * - localTreeSearch
     - :doc:`MIP Heuristics - Local tree search <MIP Heuristics/CBC_MIP_Heur_-_Local_tree_search>`
   * - maxFactor
     - :doc:`General - Refactorization interval <General/CBC_General_-_Refactorization_interval>`
   * - mixedIntegerRoundingCuts
     - :doc:`MIP Cuts - MIR cuts <MIP Cuts/CBC_MIP_Cuts_-_MIR_Cuts>`
   * - nodeStrategy
     - :doc:`MIP - Variable selection <MIP/CBC_MIP_-_Variable_Selection>`
   * - objectiveScale
     - :doc:`General - Objective scale factor <General/CBC_General_-_Objective_scale_factor>`
   * - perturbation
     - :doc:`General - Perturbation <General/CBC_General_-_Perturbation>`
   * - preprocess
     - :doc:`MIP - MIP presolve <MIP/CBC_MIP_-_MIP_presolve>`
   * - passCuts
     - :doc:`MIP Cuts - Cut passes root node <MIP Cuts/CBC_MIP_Cuts_-_Cut_passes_root_node>`
   * - passFeasibilityPump
     - :doc:`MIP Heuristics - Feasibility pump passes <MIP Heuristics/CBC_MIP_Heur_-_Feasibility_pump_passes>`
   * - passTree
     - :doc:`MIP Cuts - Cut passes tree <MIP Cuts/CBC_MIP_Cuts_-_Cut_passes_tree>`
   * - presolve
     - :doc:`Presolve - Presolve <Presolve/CBC_Presolve_-_Presolve>`
   * - preTolerance
     - :doc:`Presolve - Presolve tolerance <Presolve/CBC_Presolve_-_Presolve_tolerance>`
   * - primalPivot
     - :doc:`Simplex - Primal pivot <Simplex/CBC_Simplex_-_Primal_pivot>`
   * - primalTolerance
     - :doc:`General - Primal feasibility tolerance <General/CBC_General_-_Primal_feasibility_tol>`
   * - probingCuts
     - :doc:`MIP Cuts - Probing cuts <MIP Cuts/CBC_MIP_Cuts_-_Probing_cuts>`
   * - proximity
     - :doc:`MIP Heuristics - Proximity search <MIP Heuristics/CBC_MIP_Heur_-_Proximity_search>`
   * - reduceAndSplitCuts
     - :doc:`MIP Cuts - Reduce and split cuts <MIP Cuts/CBC_MIP_Cuts_-_Reduce_and_split_cuts>`
   * - residualCapacityCuts
     - :doc:`MIP Cuts - Residual capacity cuts <MIP Cuts/CBC_MIP_Cuts_-_Residual_capacity_cuts>`
   * - rhsScale
     - :doc:`General - RHS scale factor <General/CBC_General_-_RHS_scale_factor>`
   * - rins
     - :doc:`MIP Heuristics - RINS heuristic <MIP Heuristics/CBC_MIP_Heur_-_RINS_heuristic>`
   * - roundingHeuristic
     - :doc:`MIP Heuristics - Rounding heuristic <MIP Heuristics/CBC_MIP_Heur_-_Rounding_heuristic>`
   * - scaling
     - :doc:`General - Scaling <General/CBC_General_-_Scaling>`
   * - slogLevel
     - :doc:`Logging - Output level <Logging/CBC_Logging_-_Output_Level>`
   * - slowcutpasses
     - :doc:`MIP Cuts - Slow cut passes <MIP Cuts/CBC_MIP_Cuts_-_Slow_cut_passes>`
   * - sprintCrash
     - :doc:`General - Sifting <General/CBC_General_-_Sifting>`
   * - strongbranching
     - :doc:`MIP - Strong branching <MIP/CBC_MIP_-_Strong_branching>`
   * - trustPseudoCosts
     - :doc:`MIP - Trust pseudo costs <MIP/CBC_MIP_-_Trust_pseudo_costs>`
   * - twoMirCuts
     - :doc:`MIP Cuts - Two MIR cuts <MIP Cuts/CBC_MIP_Cuts_-_Two_MIR_cuts>`
   * - zeroHalfCuts
     - :doc:`MIP Cuts - Zero half cuts <MIP Cuts/CBC_MIP_Cuts_-_Zero_half_cuts>`
