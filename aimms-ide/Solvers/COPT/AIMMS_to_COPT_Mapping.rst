

.. _AIMMS_to_COPT_Mapping:


AIMMS to COPT Mapping
=========================

**Description** 

The table shows in the left column the AIMMS COPT options; the right column display for the AIMMS options the COPT option that is associated with it.
 		
.. list-table::

   * - **Option name in AIMMS**
     - **Option name in COPT**
   * - :ref:`Barrier - Barrier Homogeneous <option-COPT-barrier_homogeneous>`
     - BarHomogeneous
   * - :ref:`Barrier - Barrier Ordering <option-COPT-barrier_ordering>`
     - BarOrder
   * - :ref:`Barrier - Crossover <option-COPT-crossover>`
     - Crossover
   * - :ref:`General - Calculate Farkas Ray <option-COPT-calculate_farkas_ray>`
     - ReqFarkasRay
   * - :ref:`General - Dual Tolerance <option-COPT-dual_tolerance>`
     - DualTol
   * - :ref:`General - Dualize <option-COPT-dualize>`
     - Dualize
   * - :ref:`General - Feasibility Tolerance <option-COPT-feasibility_tolerance>`
     - FeasTol
   * - :ref:`General - IIS Method <option-COPT-iis_method>`
     - IISMethod
   * - :ref:`General - LP Method <option-COPT-lp_method>`
     - LpMethod
   * - :ref:`General - Matrix Tolerance <option-COPT-matrix_tolerance>`
     - MatrixTol
   * - :ref:`General - Scale <option-COPT-scale>`
     - Scaling
   * - :ref:`Logging - Log To Console <option-COPT-log_to_console>`
     - LogToConsole
   * - :ref:`MIP - Integrality Tolerance <option-COPT-integrality_tolerance>`
     - IntTol
   * - :ref:`MIP - MIP Start <option-COPT-mip_start>`
     - MipStartMode
   * - :ref:`MIP - MIP Start Node Limit <option-COPT-mip_start_node_limit>`
     - MipStartNodeLimit
   * - :ref:`MIP - Node Limit <option-COPT-node_limit>`
     - NodeLimit
   * - :ref:`MIP - Strong Branching <option-COPT-strong_branching>`
     - StrongBranching
   * - :ref:`MIP Cuts - Cut Level <option-COPT-cut_level>`
     - CutLevel
   * - :ref:`MIP Cuts - Node Cut Rounds <option-COPT-node_cut_rounds>`
     - NodeCutRounds
   * - :ref:`MIP Cuts - Root Cut Level <option-COPT-root_cut_level>`
     - RootCutLevel
   * - :ref:`MIP Cuts - Root Cut Rounds <option-COPT-root_cut_rounds>`
     - RootCutRounds
   * - :ref:`MIP Cuts - Tree Cut Level <option-COPT-tree_cut_level>`
     - TreeCutLevel
   * - :ref:`MIP Heuristics - Diving Heuristic Level <option-COPT-diving_heuristic_level>`
     - DivingHeurLevel
   * - :ref:`MIP Heuristics - Heuristic Level <option-COPT-heuristic_level>`
     - HeurLevel
   * - :ref:`MIP Heuristics - Rounding Heuristic Level <option-COPT-rounding_heuristic_level>`
     - RoundingHeurLevel
   * - :ref:`MIP Heuristics - SubMIP Heuristic Level <option-COPT-submip_heuristic_level>`
     - SubMipHeurLevel
   * - :ref:`Parallel - Barrier Thread Limit <option-COPT-barrier_thread_limit>`
     - BarThreads
   * - :ref:`Parallel - Crossover Thread Limit <option-COPT-crossover_thread_limit>`
     - CrossoverThreads
   * - :ref:`Parallel - MIP Tasks <option-COPT-mip_tasks>`
     - MipTasks
   * - :ref:`Parallel - Simplex Thread Limit <option-COPT-simplex_thread_limit>`
     - SimplexThreads
   * - :ref:`Parallel - Thread Limit <option-COPT-thread_limit>`
     - Threads
   * - :ref:`Presolve - Presolve <option-COPT-presolve>`
     - Presolve
   * - :ref:`Simplex - Objective Perturbation <option-COPT-objective_perturbation>`
     - DualPerturb
   * - :ref:`Simplex - Pricing <option-COPT-pricing>`
     - DualPrice


The table below shows Solvers General options that are mapped to COPT parameters.

.. list-table::

   * - **Option name in AIMMS**
     - **Option name in COPT**
   * - :ref:`MIP Options - MIP Absolute Optimality Tolerance <option-AIMMS-mip_absolute_optimality_tolerance>`
     - AbsGap
   * - :ref:`MIP Options - MIP Relative Optimality Tolerance <option-AIMMS-mip_relative_optimality_tolerance>`
     - RelGap
   * - :ref:`Stop Criteria - Iteration Limit <option-AIMMS-iteration_limit>`
     - BarIterLimit
   * - :ref:`Stop Criteria - Time Limit <option-AIMMS-time_limit>`
     - TimeLimit

