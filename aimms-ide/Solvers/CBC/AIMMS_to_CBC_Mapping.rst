

.. _AIMMS_to_CBC_Mapping:


AIMMS to CBC Mapping
====================

**Description** 

The table shows in the left column the AIMMS CBC options while the right column displays the associated CBC parameter.




.. list-table::

   * - **Option name in AIMMS** 
     - **Name in CBC** 
   * - :doc:`Barrier - Barrier Crossover <Barrier/CBC_Barrier_-_Barrier_crossover>` 
     - crossover
   * - :doc:`Barrier - Barrier Scaling <Barrier/CBC_Barrier_-_Barrier_Scaling>` 
     - bscale
   * - :doc:`General - Dual Feasibility Tolerance <General/CBC_General_-_Dual_Feasibility_Tol>`  
     - dualTolerance
   * - :doc:`General - LP Method <General/CBC_General_-_LP_Method>`  
     - 
   * - :doc:`General - MPS <General/CBC_General_-_MPS>`  
     - 
   * - :doc:`General - Objective Scale Factor <General/CBC_General_-_Objective_scale_factor>`  
     - objectiveScale
   * - :doc:`General - Perturbation <General/CBC_General_-_Perturbation>`  
     - perturbation
   * - :doc:`General - Primal Feasibility Tolerance <General/CBC_General_-_Primal_feasibility_tol>` 
     - primalTolerance
   * - :doc:`General - Refactorization Interval <General/CBC_General_-_Refactorization_interval>` 
     - maxFactor
   * - :doc:`General - RHS Scale Factor <General/CBC_General_-_RHS_scale_factor>` 
     - rhsScale
   * - :doc:`General - Scaling <General/CBC_General_-_Scaling>`  
     - scaling
   * - :doc:`General - Sifting <General/CBC_General_-_Sifting>`  
     - sprintCrash
   * - :doc:`Logging - MIP Print Frequency <Logging/CBC_Logging_-_MIP_print_frequency>`  
     - 
   * - :doc:`Logging - Output Level <Logging/CBC_Logging_-_Output_Level>`  
     - slogLevel
   * - :doc:`Logging - Status File <Logging/CBC_Logging_-_Status_File>`  
     - 
   * - :doc:`MIP - Increment <MIP/CBC_MIP_-_Increment>`  
     - increment
   * - :doc:`MIP - Integrality <MIP/CBC_MIP_-_Integrality>`  
     - integerTolerance
   * - :doc:`MIP - MIP Basis <MIP/CBC_MIP_-_MIP_Basis>`  
     - 
   * - :doc:`MIP - MIP Presolve <MIP/CBC_MIP_-_MIP_presolve>`  
     - preprocess
   * - :doc:`MIP - MIP Start <MIP/CBC_MIP_-_MIP_Start>`  
     - 
   * - :doc:`MIP - Node Selection <MIP/CBC_MIP_-_Node_selection>`  
     - nodeStrategy
   * - :doc:`MIP - Strong Branching <MIP/CBC_MIP_-_Strong_branching>`  
     - strongbranching
   * - :doc:`MIP - Trust Pseudo Costs <MIP/CBC_MIP_-_Trust_pseudo_costs>`  
     - trustPseudoCosts
   * - :doc:`MIP - Variable Selection <MIP/CBC_MIP_-_Variable_Selection>`  
     - costStrategy
   * - :doc:`MIP Cuts - Clique Cuts <MIP Cuts/CBC_MIP_Cuts_-_Clique_Cuts>`  
     - cliqueCuts
   * - :doc:`MIP Cuts - Cut Depth <MIP Cuts/CBC_MIP_Cuts_-_Cut_Depth>` 
     - cutDepth
   * - :doc:`MIP Cuts - Cut Passes Root Node <MIP Cuts/CBC_MIP_Cuts_-_Cut_passes_root_node>` 
     - passCuts
   * - :doc:`MIP Cuts - Cut Passes Tree <MIP Cuts/CBC_MIP_Cuts_-_Cut_passes_tree>` 
     - passTree
   * - :doc:`MIP Cuts - Flow Cover Cuts <MIP Cuts/CBC_MIP_Cuts_-_Flow_Cover_Cuts>` 
     - flowCoverCuts
   * - :doc:`MIP Cuts - Global Cut Control <MIP Cuts/CBC_MIP_Cuts_-_Global_Cut_Control>`  
     - cuts
   * - :doc:`MIP Cuts - Gomory Cuts <MIP Cuts/CBC_MIP_Cuts_-_Gomory_Cuts>` 
     - gomoryCuts
   * - :doc:`MIP Cuts - Knapsack Cuts <MIP Cuts/CBC_MIP_Cuts_-_Knapsack_Cuts>` 
     - knapsackCuts
   * - :doc:`MIP Cuts - Lift and Project Cuts <MIP Cuts/CBC_MIP_Cuts_-_Lift_and_Project_Cuts>` 
     - liftAndProjectCuts
   * - :doc:`MIP Cuts - MIR Cuts <MIP Cuts/CBC_MIP_Cuts_-_MIR_Cuts>`  
     - mixedIntegerRoundingCuts
   * - :doc:`MIP Cuts - Probing Cuts <MIP Cuts/CBC_MIP_Cuts_-_Probing_cuts>`  
     - probingCuts
   * - :doc:`MIP Cuts - Reduce and Split Cuts <MIP Cuts/CBC_MIP_Cuts_-_Reduce_and_split_cuts>`  
     - reduceAndSplitCuts
   * - :doc:`MIP Cuts - Residual Capacity Cuts <MIP Cuts/CBC_MIP_Cuts_-_Residual_capacity_cuts>`  
     - residualCapacityCuts
   * - :doc:`MIP Cuts - Slow Cut Passes <MIP Cuts/CBC_MIP_Cuts_-_Slow_cut_passes>`  
     - slowcutpasses
   * - :doc:`MIP Cuts - Two MIR Cuts <MIP Cuts/CBC_MIP_Cuts_-_Two_MIR_cuts>`  
     - twoMirCuts
   * - :doc:`MIP Cuts - Zero Half Cuts <MIP Cuts/CBC_MIP_Cuts_-_Zero_half_cuts>`  
     - zeroHalfCuts
   * - :doc:`MIP Heuristics - Combine Solutions <MIP Heuristics/CBC_MIP_Heur_-_Combine_solutions>`  
     - combineSolutions
   * - :doc:`MIP Heuristics - Feasibility Pump <MIP Heuristics/CBC_MIP_Heur_-_Feasibility_pump>`  
     - feasibilityPump
   * - :doc:`MIP Heuristics - Feasibility Pump Passes <MIP Heuristics/CBC_MIP_Heur_-_Feasibility_pump_passes>`  
     - passFeasibilityPump
   * - :doc:`MIP Heuristics - Greedy Heuristic <MIP Heuristics/CBC_MIP_Heur_-_Greedy_heuristic>`  
     - greedyHeuristic
   * - :doc:`MIP Heuristics - Heuristics <MIP Heuristics/CBC_MIP_Heur_-_Heuristics>`  
     - heuristicsOnOff
   * - :doc:`MIP Heuristics - Local Tree Search <MIP Heuristics/CBC_MIP_Heur_-_Local_tree_search>`  
     - localTreeSearch
   * - :doc:`MIP Heuristics - Proximity Search <MIP Heuristics/CBC_MIP_Heur_-_Proximity_search>` 
     - proximity
   * - :doc:`MIP Heuristics - RINS Heuristic <MIP Heuristics/CBC_MIP_Heur_-_RINS_heuristic>`  
     - rins
   * - :doc:`MIP Heuristics - Rounding Heuristic <MIP Heuristics/CBC_MIP_Heur_-_Rounding_heuristic>`  
     - roundingHeuristic
   * - :doc:`Presolve - Presolve <Presolve/CBC_Presolve_-_Presolve>` 
     - presolve
   * - :doc:`Presolve - Presolve Tolerance <Presolve/CBC_Presolve_-_Presolve_tolerance>`  
     - preTolerance
   * - :doc:`Simplex - Crash <Simplex/CBC_Simplex_-_Crash>` 
     - crash	
   * - :doc:`Simplex - Dual Pivot <Simplex/CBC_Simplex_-_Dual_pivot>` 
     - dualPivot
   * - :doc:`Simplex - Idiot Crash <Simplex/CBC_Simplex_-_Idiot_crash>` 
     - idiotCrash
   * - :doc:`Simplex - Primal Pivot <Simplex/CBC_Simplex_-_Primal_pivot>`  
     - primalPivot


				

