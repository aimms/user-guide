

.. _CBC_to_AIMMS_Mapping:


CBC to AIMMS Mapping
====================

**Description** 

The table shows in the left column the parameters from CBC that can be set in AIMMS; the right column displays for each CBC parameter the associated AIMMS option.



.. list-table::

   * - **Name in CBC**
     - **Option name in AIMMS**
   * - bscale
     - :doc:`Barrier - Barrier Scaling <Barrier/CBC_Barrier_-_Barrier_Scaling>`
   * - cliqueCuts
     - :doc:`MIP Cuts - Clique Cuts <MIP Cuts/CBC_MIP_Cuts_-_Clique_Cuts>`
   * - combineSolutions
     - :doc:`MIP Heuristics - Combine Solutions <MIP Heuristics/CBC_MIP_Heur_-_Combine_solutions>`
   * - costStrategy
     - :doc:`MIP - Variable Selection <MIP/CBC_MIP_-_Variable_Selection>`
   * - crash
     - :doc:`Simplex - Crash <Simplex/CBC_Simplex_-_Crash>`
   * - crossover
     - :doc:`Barrier - Barrier Crossover <Barrier/CBC_Barrier_-_Barrier_crossover>`
   * - cutDepth
     - :doc:`MIP Cuts - Cut Depth <MIP Cuts/CBC_MIP_Cuts_-_Cut_Depth>`
   * - cuts
     - :doc:`MIP Cuts - Global Cut Control <MIP Cuts/CBC_MIP_Cuts_-_Global_Cut_Control>`
   * - dualTolerance
     - :doc:`General - Dual Feasibility Tolerance <General/CBC_General_-_Dual_Feasibility_Tol>`
   * - dualPivot
     - :doc:`Simplex - Dual Pivot <Simplex/CBC_Simplex_-_Dual_pivot>`
   * - feasibilityPump
     - :doc:`MIP Heuristics - Feasibility Pump <MIP Heuristics/CBC_MIP_Heur_-_Feasibility_pump>`
   * - flowCoverCuts
     - :doc:`MIP Cuts - Flow Cover Cuts <MIP Cuts/CBC_MIP_Cuts_-_Flow_Cover_Cuts>`
   * - gomoryCuts
     - :doc:`MIP Cuts - Gomory Cuts <MIP Cuts/CBC_MIP_Cuts_-_Gomory_Cuts>`
   * - greedyHeuristic
     - :doc:`MIP Heuristics - Greedy Heuristic <MIP Heuristics/CBC_MIP_Heur_-_Greedy_heuristic>`
   * - heuristicsOnOff
     - :doc:`MIP Heuristics - Heuristics <MIP Heuristics/CBC_MIP_Heur_-_Heuristics>`
   * - idiotCrash
     - :doc:`Simplex - Idiot Crash <Simplex/CBC_Simplex_-_Idiot_crash>`
   * - increment
     - :doc:`MIP - Increment <MIP/CBC_MIP_-_Increment>`
   * - integerTolerance
     - :doc:`MIP - Integrality <MIP/CBC_MIP_-_Integrality>`
   * - knapsackCuts
     - :doc:`MIP Cuts - Knapsack Cuts <MIP Cuts/CBC_MIP_Cuts_-_Knapsack_Cuts>`
   * - liftAndProjectCuts
     - :doc:`MIP Cuts - Lift and Project Cuts <MIP Cuts/CBC_MIP_Cuts_-_Lift_and_Project_Cuts>`
   * - localTreeSearch
     - :doc:`MIP Heuristics - Local Tree Search <MIP Heuristics/CBC_MIP_Heur_-_Local_tree_search>`
   * - maxFactor
     - :doc:`General - Refactorization Interval <General/CBC_General_-_Refactorization_interval>`
   * - mixedIntegerRoundingCuts
     - :doc:`MIP Cuts - MIR Cuts <MIP Cuts/CBC_MIP_Cuts_-_MIR_Cuts>`
   * - nodeStrategy
     - :doc:`MIP - Variable Selection <MIP/CBC_MIP_-_Variable_Selection>`
   * - objectiveScale
     - :doc:`General - Objective Scale Factor <General/CBC_General_-_Objective_scale_factor>`
   * - perturbation
     - :doc:`General - Perturbation <General/CBC_General_-_Perturbation>`
   * - preprocess
     - :doc:`MIP - MIP Presolve <MIP/CBC_MIP_-_MIP_presolve>`
   * - passCuts
     - :doc:`MIP Cuts - Cut Passes Root Node <MIP Cuts/CBC_MIP_Cuts_-_Cut_passes_root_node>`
   * - passFeasibilityPump
     - :doc:`MIP Heuristics - Feasibility Pump Passes <MIP Heuristics/CBC_MIP_Heur_-_Feasibility_pump_passes>`
   * - passTree
     - :doc:`MIP Cuts - Cut Passes Tree <MIP Cuts/CBC_MIP_Cuts_-_Cut_passes_tree>`
   * - presolve
     - :doc:`Presolve - Presolve <Presolve/CBC_Presolve_-_Presolve>`
   * - preTolerance
     - :doc:`Presolve - Presolve Tolerance <Presolve/CBC_Presolve_-_Presolve_tolerance>`
   * - primalPivot
     - :doc:`Simplex - Primal Pivot <Simplex/CBC_Simplex_-_Primal_pivot>`
   * - primalTolerance
     - :doc:`General - Primal Feasibility Tolerance <General/CBC_General_-_Primal_feasibility_tol>`
   * - probingCuts
     - :doc:`MIP Cuts - Probing Cuts <MIP Cuts/CBC_MIP_Cuts_-_Probing_cuts>`
   * - proximity
     - :doc:`MIP Heuristics - Proximity Search <MIP Heuristics/CBC_MIP_Heur_-_Proximity_search>`
   * - reduceAndSplitCuts
     - :doc:`MIP Cuts - Reduce and Split Cuts <MIP Cuts/CBC_MIP_Cuts_-_Reduce_and_split_cuts>`
   * - residualCapacityCuts
     - :doc:`MIP Cuts - Residual Capacity Cuts <MIP Cuts/CBC_MIP_Cuts_-_Residual_capacity_cuts>`
   * - rhsScale
     - :doc:`General - RHS Scale Factor <General/CBC_General_-_RHS_scale_factor>`
   * - rins
     - :doc:`MIP Heuristics - RINS Heuristic <MIP Heuristics/CBC_MIP_Heur_-_RINS_heuristic>`
   * - roundingHeuristic
     - :doc:`MIP Heuristics - Rounding Heuristic <MIP Heuristics/CBC_MIP_Heur_-_Rounding_heuristic>`
   * - scaling
     - :doc:`General - Scaling <General/CBC_General_-_Scaling>`
   * - slogLevel
     - :doc:`Logging - Output Level <Logging/CBC_Logging_-_Output_Level>`
   * - slowcutpasses
     - :doc:`MIP Cuts - Slow Cut Passes <MIP Cuts/CBC_MIP_Cuts_-_Slow_cut_passes>`
   * - sprintCrash
     - :doc:`General - Sifting <General/CBC_General_-_Sifting>`
   * - strongbranching
     - :doc:`MIP - Strong Branching <MIP/CBC_MIP_-_Strong_branching>`
   * - trustPseudoCosts
     - :doc:`MIP - Trust Pseudo Costs <MIP/CBC_MIP_-_Trust_pseudo_costs>`
   * - twoMirCuts
     - :doc:`MIP Cuts - Two MIR Cuts <MIP Cuts/CBC_MIP_Cuts_-_Two_MIR_cuts>`
   * - zeroHalfCuts
     - :doc:`MIP Cuts - Zero Half Cuts <MIP Cuts/CBC_MIP_Cuts_-_Zero_half_cuts>`
