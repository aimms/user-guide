

.. _AIMMS_to_CBC_Mapping:


AIMMS to CBC Mapping
====================

**Description** 

The table shows in the left column the AIMMS CBC options while the right column displays the associated CBC parameter.




.. list-table::

   * - **Option name in AIMMS** 
     - **Name in CBC** 
   * - :doc:`Barrier - Barrier crossover <Barrier/CBC_Barrier_-_Barrier_crossover>` 
     - crossover
   * - :doc:`Barrier - Barrier scaling <Barrier/CBC_Barrier_-_Barrier_Scaling>` 
     - bscale
   * - :doc:`General - Dual feasibility tolerance <General/CBC_General_-_Dual_Feasibility_Tol>`  
     - dualTolerance
   * - :doc:`General - LP method <General/CBC_General_-_LP_Method>`  
     - 
   * - :doc:`General - MPS <General/CBC_General_-_MPS>`  
     - 
   * - :doc:`General - Objective scale factor <General/CBC_General_-_Objective_scale_factor>`  
     - objectiveScale
   * - :doc:`General - Perturbation <General/CBC_General_-_Perturbation>`  
     - perturbation
   * - :doc:`General - Primal feasibility tolerance <General/CBC_General_-_Primal_feasibility_tol>` 
     - primalTolerance
   * - :doc:`General - Refactorization interval <General/CBC_General_-_Refactorization_interval>` 
     - maxFactor
   * - :doc:`General - RHS scale factor <General/CBC_General_-_RHS_scale_factor>` 
     - rhsScale
   * - :doc:`General - Scaling <General/CBC_General_-_Scaling>`  
     - scaling
   * - :doc:`General - Sifting <General/CBC_General_-_Sifting>`  
     - sprintCrash
   * - :doc:`Logging - MIP print frequency <Logging/CBC_Logging_-_MIP_print_frequency>`  
     - 
   * - :doc:`Logging - Output level <Logging/CBC_Logging_-_Output_Level>`  
     - slogLevel
   * - :doc:`Logging - Status file <Logging/CBC_Logging_-_Status_File>`  
     - 
   * - :doc:`MIP - Increment <MIP/CBC_MIP_-_Increment>`  
     - increment
   * - :doc:`MIP - Integrality <MIP/CBC_MIP_-_Integrality>`  
     - integerTolerance
   * - :doc:`MIP - MIP basis <MIP/CBC_MIP_-_MIP_Basis>`  
     - 
   * - :doc:`MIP - MIP presolve <MIP/CBC_MIP_-_MIP_presolve>`  
     - preprocess
   * - :doc:`MIP - MIP start <MIP/CBC_MIP_-_MIP_Start>`  
     - 
   * - :doc:`MIP - Node selection <MIP/CBC_MIP_-_Node_selection>`  
     - nodeStrategy
   * - :doc:`MIP - Strong branching <MIP/CBC_MIP_-_Strong_branching>`  
     - strongbranching
   * - :doc:`MIP - Trust pseudo costs <MIP/CBC_MIP_-_Trust_pseudo_costs>`  
     - trustPseudoCosts
   * - :doc:`MIP - Variable selection <MIP/CBC_MIP_-_Variable_Selection>`  
     - costStrategy
   * - :doc:`MIP Cuts - Clique cuts <MIP Cuts/CBC_MIP_Cuts_-_Clique_Cuts>`  
     - cliqueCuts
   * - :doc:`MIP Cuts - Cut depth <MIP Cuts/CBC_MIP_Cuts_-_Cut_Depth>` 
     - cutDepth
   * - :doc:`MIP Cuts - Cut passes root node <MIP Cuts/CBC_MIP_Cuts_-_Cut_passes_root_node>` 
     - passCuts
   * - :doc:`MIP Cuts - Cut passes tree <MIP Cuts/CBC_MIP_Cuts_-_Cut_passes_tree>` 
     - passTree
   * - :doc:`MIP Cuts - Flow cover cuts <MIP Cuts/CBC_MIP_Cuts_-_Flow_Cover_Cuts>` 
     - flowCoverCuts
   * - :doc:`MIP Cuts - Global cut control <MIP Cuts/CBC_MIP_Cuts_-_Global_Cut_Control>`  
     - cuts
   * - :doc:`MIP Cuts - Gomory cuts <MIP Cuts/CBC_MIP_Cuts_-_Gomory_Cuts>` 
     - gomoryCuts
   * - :doc:`MIP Cuts - Knapsack cuts <MIP Cuts/CBC_MIP_Cuts_-_Knapsack_Cuts>` 
     - knapsackCuts
   * - :doc:`MIP Cuts - Lift and project cuts <MIP Cuts/CBC_MIP_Cuts_-_Lift_and_Project_Cuts>` 
     - liftAndProjectCuts
   * - :doc:`MIP Cuts - MIR cuts <MIP Cuts/CBC_MIP_Cuts_-_MIR_Cuts>`  
     - mixedIntegerRoundingCuts
   * - :doc:`MIP Cuts - Probing cuts <MIP Cuts/CBC_MIP_Cuts_-_Probing_cuts>`  
     - probingCuts
   * - :doc:`MIP Cuts - Reduce and split cuts <MIP Cuts/CBC_MIP_Cuts_-_Reduce_and_split_cuts>`  
     - reduceAndSplitCuts
   * - :doc:`MIP Cuts - Residual capacity cuts <MIP Cuts/CBC_MIP_Cuts_-_Residual_capacity_cuts>`  
     - residualCapacityCuts
   * - :doc:`MIP Cuts - Slow cut passes <MIP Cuts/CBC_MIP_Cuts_-_Slow_cut_passes>`  
     - slowcutpasses
   * - :doc:`MIP Cuts - Two MIR cuts <MIP Cuts/CBC_MIP_Cuts_-_Two_MIR_cuts>`  
     - twoMirCuts
   * - :doc:`MIP Cuts - Zero half cuts <MIP Cuts/CBC_MIP_Cuts_-_Zero_half_cuts>`  
     - zeroHalfCuts
   * - :doc:`MIP Heuristics - Combine solutions <MIP Heuristics/CBC_MIP_Heur_-_Combine_solutions>`  
     - combineSolutions
   * - :doc:`MIP Heuristics - Feasibility pump <MIP Heuristics/CBC_MIP_Heur_-_Feasibility_pump>`  
     - feasibilityPump
   * - :doc:`MIP Heuristics - Feasibility pump passes <MIP Heuristics/CBC_MIP_Heur_-_Feasibility_pump_passes>`  
     - passFeasibilityPump
   * - :doc:`MIP Heuristics - Greedy heuristic <MIP Heuristics/CBC_MIP_Heur_-_Greedy_heuristic>`  
     - greedyHeuristic
   * - :doc:`MIP Heuristics - Heuristics <MIP Heuristics/CBC_MIP_Heur_-_Heuristics>`  
     - heuristicsOnOff
   * - :doc:`MIP Heuristics - Local tree search <MIP Heuristics/CBC_MIP_Heur_-_Local_tree_search>`  
     - localTreeSearch
   * - :doc:`MIP Heuristics - Proximity search <MIP Heuristics/CBC_MIP_Heur_-_Proximity_search>` 
     - proximity
   * - :doc:`MIP Heuristics - RINS heuristic <MIP Heuristics/CBC_MIP_Heur_-_RINS_heuristic>`  
     - rins
   * - :doc:`MIP Heuristics - Rounding heuristic <MIP Heuristics/CBC_MIP_Heur_-_Rounding_heuristic>`  
     - roundingHeuristic
   * - :doc:`Presolve - Presolve <Presolve/CBC_Presolve_-_Presolve>` 
     - presolve
   * - :doc:`Presolve - Presolve tolerance <Presolve/CBC_Presolve_-_Presolve_tolerance>`  
     - preTolerance
   * - :doc:`Simplex - Crash <Simplex/CBC_Simplex_-_Crash>` 
     - crash	
   * - :doc:`Simplex - Dual pivot <Simplex/CBC_Simplex_-_Dual_pivot>` 
     - dualPivot
   * - :doc:`Simplex - Idiot crash <Simplex/CBC_Simplex_-_Idiot_crash>` 
     - idiotCrash
   * - :doc:`Simplex - Primal pivot <Simplex/CBC_Simplex_-_Primal_pivot>`  
     - primalPivot


				

