

.. _AIMMS_to_XA_Mapping:


AIMMS to XA Mapping
===================

**Description** 

The table shows in the left column the AIMMS XA options; the right column displays for the AIMMS options the XA parameter that is associated with it.

.. list-table::

   * - **Option name in AIMMS**
     - **Name in XA**
   * - :ref:`Advanced - Dual Activity Tolerance <option-XA-dual_activity_tolerance>`
     - SET TOLERANCE DUAL
   * - :ref:`Advanced - Maximal Absolute Pivot Value <option-XA-maximal_absolute_pivot_value>`
     - SET REJPIVOT
   * - :ref:`Advanced - Minimal Absolute Pivot Value <option-XA-minimal_absolute_pivot_value>`
     - SET YPIVOT
   * - :ref:`Advanced - Perturbate <option-XA-perturbate>`
     - SET PERTURBATE
   * - :ref:`Advanced - Primal Activity Tolerance <option-XA-primal_activity_tolerance>`
     - SET TOLERANCE PRIMAL
   * - :ref:`Advanced - Size of Smallest Element <option-XA-size_of_smallest_element>`
     - SET ELEMSIZE
   * - :ref:`General - Crash <option-XA-crash>`
     - SET CRASH
   * - :ref:`General - Force <option-XA-force>`
     - CONFLICT
   * - :ref:`General - LP Method <option-XA-lp_method>`
     - SET BARRIER
   * - :ref:`General - MPS <option-XA-mps>`
     - TOMPS
   * - :ref:`General - Presolve <option-XA-presolve>`
     - SET ELIMINATE
   * - :ref:`General - Presolve Activity Types <option-XA-presolve_activity_types>`
     - PRESOLVE
   * - :ref:`General - Restart <option-XA-restart>`
     - SET RESTART
   * - :ref:`General - Restart File Number <option-XA-restart_file_number>`
     - 
   * - :ref:`General - Scale <option-XA-scale>`
     - SET SCALE
   * - :ref:`General - Solution File <option-XA-solution_file>`
     -
   * - :ref:`General - Windows Friendly <option-XA-windows_friendly>`
     - SET WINFRIENDLY
   * - :ref:`Logging - Node Log <option-XA-node_log>`
     -
   * - :ref:`Logging - Simplex Log <option-XA-simplex_log>`
     -
   * - :ref:`Memory - Extra Memory <option-XA-extra_memory>`
     -
   * - :ref:`Memory - Minimal Memory Size <option-XA-minimal_memory_size>`
     -
   * - :ref:`MIP - Basis in Memory <option-XA-basis_in_memory>`
     - SET BASISMEMORY
   * - :ref:`MIP - Dual Simplex <option-XA-dual_simplex>`
     - SET DUALSIMPLEX
   * - :ref:`MIP - Lower Integer Tolerance <option-XA-lower_integer_tolerance>`
     - SET LTOLERANCE
   * - :ref:`MIP - Maximal Number of Generated Nodes <option-XA-maximal_number_of_generated_nodes>`
     - SET LIMITNODES
   * - :ref:`MIP - Maximal Number of Nodes <option-XA-maximal_number_of_nodes>`
     - SET MAXNODES
   * - :ref:`MIP - MIP Basis <option-XA-mip_basis>`
     -
   * - :ref:`MIP - MIP Branch Order <option-XA-mip_branch_order>`
     - PRIORITY
   * - :ref:`MIP - MIP Postsolve <option-XA-mip_postsolve>`
     -
   * - :ref:`MIP - MIP Strategy <option-XA-mip_strategy>`
     - STRATEGY
   * - :ref:`MIP - MIP Strategy Branching Priorities <option-XA-mip_strategy_branching_priorities>`
     - STRATEGY
   * - :ref:`MIP - MIP Strategy Estimate Integer Solution <option-XA-mip_strategy_estimate_integer_solution>`
     - STRATEGY
   * - :ref:`MIP - MIP Strategy Split Node List <option-XA-mip_strategy_split_node_list>`
     - STRATEGY
   * - :ref:`MIP - MIP Update <option-XA-mip_update>`
     -
   * - :ref:`MIP - Percentage Fixed Integer Variables <option-XA-percentage_fixed_integer_variables>`
     - SET INTPCT
   * - :ref:`MIP - Selection of Nodes <option-XA-selection_of_nodes>`
     - SET RUNNER
   * - :ref:`MIP - Stop After <option-XA-stop_after>`
     - STOPAFTER
   * - :ref:`MIP - Stop Unchanged <option-XA-stop_unchanged>`
     - STOPUNCHANGED
   * - :ref:`MIP - Tree Depth <option-XA-tree_depth>`
     - TREEDEPTH
   * - :ref:`MIP - Tree Time <option-XA-tree_time>`
     - TREETIME
   * - :ref:`MIP - Upper Integer Tolerance <option-XA-upper_integer_tolerance>`
     - SET UTOLERANCE
   * - :ref:`Simplex - Degenerate Pivots <option-XA-degenerate_pivots>`
     - SET DEGENITER
   * - :ref:`Simplex - Markowitz <option-XA-markowitz>`
     - SET MARKOWITZ
   * - :ref:`Simplex - Pricing <option-XA-pricing>`
     - SET PRICING
   * - :ref:`Simplex - Primal Infeasibility <option-XA-primal_infeasibility>`
     - SET XTOZERO
   * - :ref:`Simplex - Reduced Cost <option-XA-reduced_cost>`
     - SET REDUCEDCOST
   * - :ref:`Simplex - Reinvert Frequency <option-XA-reinvert_frequency>`
     - SET REINVERTFREQ
