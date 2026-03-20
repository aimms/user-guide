

.. _AIMMS_to_XA_Mapping:


AIMMS to XA Mapping
===================

**Description** 

The table shows in the left column the AIMMS XA options; the right column displays for the AIMMS options the XA parameter that is associated with it.

.. list-table::

   * - **Option name in AIMMS**
     - **Name in XA**
   * - :doc:`Advanced - Dual Activity Tolerance <Advanced/XA_Advanced_-_Dual_Activity_Toler>`
     - SET TOLERANCE DUAL
   * - :doc:`Advanced - Maximal Absolute Pivot Value <Advanced/XA_Advanced_-_Maximal_Absolute_Pi>`
     - SET REJPIVOT
   * - :doc:`Advanced - Minimal Absolute Pivot Value <Advanced/XA_Advanced_-_Minimal_Absolute_Pi>`
     - SET YPIVOT
   * - :doc:`Advanced - Perturbate <Advanced/XA_Advanced_-_Perturbate>`
     - SET PERTURBATE
   * - :doc:`Advanced - Primal Activity Tolerance <Advanced/XA_Advanced_-_Primal_Activity_Tol>`
     - SET TOLERANCE PRIMAL
   * - :doc:`Advanced - Size of Smallest Element <Advanced/XA_Advanced_-_Size_of_Smallest_El>`
     - SET ELEMSIZE
   * - :doc:`General - Crash <General/XA_General_-_Crash>`
     - SET CRASH
   * - :doc:`General - Force <General/XA_General_-_Force>`
     - CONFLICT
   * - :doc:`General - LP Method <General/XA_General_-_LP_Method>`
     - SET BARRIER
   * - :doc:`General - MPS <General/XA_General_-_MPS>`
     - TOMPS
   * - :doc:`General - Presolve <General/XA_General_-_Presolve>`
     - SET ELIMINATE
   * - :doc:`General - Presolve Activity Types <General/XA_General_-_Presolve_Activity_Types>`
     - PRESOLVE
   * - :doc:`General - Restart <General/XA_General_-_Restart>`
     - SET RESTART
   * - :doc:`General - Restart File Number <General/XA_General_-_Restart_File_Number>`
     - 
   * - :doc:`General - Scale <General/XA_General_-_Scale>`
     - SET SCALE
   * - :doc:`General - Solution File <General/XA_General_-_Solution_File>`
     -
   * - :doc:`General - Windows Friendly <General/XA_General_-_Windows_Friendly>`
     - SET WINFRIENDLY
   * - :doc:`Logging - Node Log <Logging/XA_Logging_-_Node_Log>`
     -
   * - :doc:`Logging - Simplex Log <Logging/XA_Logging_-_Simplex_Log>`
     -
   * - :doc:`Memory - Extra Memory <Memory/XA_Memory_-_Extra_Memory>`
     -
   * - :doc:`Memory - Minimal Memory Size <Memory/XA_Memory_-_Minimal_Memory_Size>`
     -
   * - :doc:`MIP - Basis in Memory <MIP/XA_MIP_-_Basis_in_Memory>`
     - SET BASISMEMORY
   * - :doc:`MIP - Dual Simplex <MIP/XA_MIP_-_Dual_Simplex>`
     - SET DUALSIMPLEX
   * - :doc:`MIP - Lower Integer Tolerance <MIP/XA_MIP_-_Lower_Integer_Tolerance>`
     - SET LTOLERANCE
   * - :doc:`MIP - Maximal Number of Generated Nodes <MIP/XA_MIP_-_Maximal_Number_of_Genera>`
     - SET LIMITNODES
   * - :doc:`MIP - Maximal Number of Nodes <MIP/XA_MIP_-_Maximal_Number_of_Nodes>`
     - SET MAXNODES
   * - :doc:`MIP - MIP Basis <MIP/XA_MIP_-_MIP_Basis>`
     -
   * - :doc:`MIP - MIP Branch Order <MIP/XA_MIP_-_MIP_Branch_Order>`
     - PRIORITY
   * - :doc:`MIP - MIP Postsolve <MIP/XA_MIP_-_MIP_Postsolve>`
     -
   * - :doc:`MIP - MIP Strategy <MIP/XA_MIP_-_MIP_Strategy>`
     - STRATEGY
   * - :doc:`MIP - MIP Strategy Branching Priorities <MIP/XA_MIP_-_MIP_Strategy_Branching_P>`
     - STRATEGY
   * - :doc:`MIP - MIP Strategy Estimate Integer Solution <MIP/XA_MIP_-_MIP_Strategy_Estimate_In>`
     - STRATEGY
   * - :doc:`MIP - MIP Strategy Split Node List <MIP/XA_MIP_-_MIP_Strategy_Split_Node_>`
     - STRATEGY
   * - :doc:`MIP - MIP Update <MIP/XA_MIP_-_MIP_Update>`
     -
   * - :doc:`MIP - Percentage Fixed Integer Variables <MIP/XA_MIP_-_Percentage_Fixed_Integer>`
     - SET INTPCT
   * - :doc:`MIP - Selection of Nodes <MIP/XA_MIP_-_Selection_of_Nodes>`
     - SET RUNNER
   * - :doc:`MIP - Stop After <MIP/XA_MIP_-_Stop_After>`
     - STOPAFTER
   * - :doc:`MIP - Stop Unchanged <MIP/XA_MIP_-_Stop_Unchanged>`
     - STOPUNCHANGED
   * - :doc:`MIP - Tree Depth <MIP/XA_MIP_-_Tree_Depth>`
     - TREEDEPTH
   * - :doc:`MIP - Tree Time <MIP/XA_MIP_-_Tree_Time>`
     - TREETIME
   * - :doc:`MIP - Upper Integer Tolerance <MIP/XA_MIP_-_Upper_Integer_Tolerance>`
     - SET UTOLERANCE
   * - :doc:`Simplex - Degenerate Pivots <Simplex/XA_Simplex_-_Degenerate_Pivots>`
     - SET DEGENITER
   * - :doc:`Simplex - Markowitz <Simplex/XA_Simplex_-_Markowitz>`
     - SET MARKOWITZ
   * - :doc:`Simplex - Pricing <Simplex/XA_Simplex_-_Pricing>`
     - SET PRICING
   * - :doc:`Simplex - Primal Infeasibility <Simplex/XA_Simplex_-_Primal_Infeasibility>`
     - SET XTOZERO
   * - :doc:`Simplex - Reduced Cost <Simplex/XA_Simplex_-_Reduced_Cost>`
     - SET REDUCEDCOST
   * - :doc:`Simplex - Reinvert Frequency <Simplex/XA_Simplex_-_Reinvert_Frequency>`
     - SET REINVERTFREQ
