

.. _XA_to_AIMMS_Mappings:


XA to AIMMS Mapping
===================

**Description** 

The table shows in the left column the parameters from XA that can be set in AIMMS; the right column displays for each XA parameter the associated AIMMS option.

.. list-table::

   * - **Name in XA**
     - **Option name in AIMMS**
   * - CONFLICT
     - :ref:`option-XA-force`
   * - PRESOLVE
     - :ref:`option-XA-presolve_activity_types`
   * - PRIORITY
     - :ref:`option-XA-mip_branch_order`
   * - SET BARRIER
     - :ref:`option-XA-lp_method`
   * - SET BASISMEMORY
     - :ref:`option-XA-basis_in_memory`
   * - SET CRASH
     - :ref:`option-XA-crash`
   * - SET DEGENITER
     - :ref:`option-XA-degenerate_pivots`
   * - SET DUALSIMPLEX
     - :ref:`option-XA-dual_simplex`
   * - SET ELEMSIZE
     - :ref:`option-XA-size_of_smallest_element`
   * - SET ELIMINATE
     - :ref:`option-XA-presolve`
   * - SET INTPCT
     - :ref:`option-XA-percentage_fixed_integer_variables`
   * - SET LIMITNODES
     - :ref:`option-XA-maximal_number_of_generated_nodes`
   * - SET LTOLERANCE
     - :ref:`option-XA-lower_integer_tolerance`
   * - SET MARKOWITZ
     - :ref:`option-XA-markowitz`
   * - SET MAXNODES
     - :ref:`option-XA-maximal_number_of_nodes`
   * - SET PERTURBATE
     - :ref:`option-XA-perturbate`
   * - SET PRICING
     - :ref:`option-XA-pricing`
   * - SET REDUCEDCOST
     - :ref:`option-XA-reduced_cost`
   * - SET REINVERTFREQ
     - :ref:`option-XA-reinvert_frequency`
   * - SET REJPIVOT
     - :ref:`option-XA-maximal_absolute_pivot_value`
   * - SET RESTART
     - :ref:`option-XA-restart`
   * - SET RUNNER
     - :ref:`option-XA-selection_of_nodes`
   * - SET SCALE
     - :ref:`option-XA-scale`
   * - SET TOLERANCE DUAL
     - :ref:`option-XA-dual_activity_tolerance`
   * - SET TOLERANCE PRIMAL
     - :ref:`option-XA-primal_activity_tolerance`
   * - SET UTOLERANCE
     - :ref:`option-XA-upper_integer_tolerance`
   * - SET WINFRIENDLY
     - :ref:`option-XA-windows_friendly`
   * - SET XTOZERO
     - :ref:`option-XA-primal_infeasibility`
   * - SET YPIVOT
     - :ref:`option-XA-minimal_absolute_pivot_value`
   * - STOPAFTER
     - :ref:`option-XA-stop_after`
   * - STOPUNCHANGED
     - :ref:`option-XA-stop_unchanged`
   * - STRATEGY
     - :ref:`option-XA-mip_strategy`
   * - 
     - :ref:`option-XA-mip_strategy_branching_priorities`
   * - 
     - :ref:`option-XA-mip_strategy_estimate_integer_solution`
   * - 
     - :ref:`option-XA-mip_strategy_split_node_list`
   * - TOMPS
     - :ref:`option-XA-mps`
   * - TREEDEPTH
     - :ref:`option-XA-tree_depth`
   * - TREETIME
     - :ref:`option-XA-tree_time`
