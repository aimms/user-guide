

.. _AIMMS_to_CONOPT_Mapping:


AIMMS to CONOPT Mapping
=======================

**Description** 

The table shows in the left column the AIMMS CONOPT options; 
the right column displays for the AIMMS option 
the CONOPT parameter that is associated with it.

.. list-table::

   * - **Option name in AIMMS**
     - **Name in CONOPT**
   * - :doc:`Advanced - Box Size Factor Linear Variables <Advanced/CONOPT_Advanced_-_Box_Size_Factor_Linear_Var>`
     - RTBOXF
   * - :doc:`Advanced - Box Size Tolerance <Advanced/CONOPT_Advanced_-_Box_Size_Tolerance>`
     - RTBOX
   * - :doc:`Advanced - Box Size Tolerance Linear <Advanced/CONOPT_Advanced_-_Box_Size_Tolerance_Linear>`
     - RTBOXL
   * - :doc:`Advanced - Fixed Variables Tolerance Derived Bounds <Advanced/CONOPT_Advanced_-_Fixed_Var_Tol_Derived_Bounds>`
     - RTBNDT
   * - :doc:`Advanced - Fixed Variables Tolerance Initial Bounds <Advanced/CONOPT_Advanced_-_Fixed_Var_Tol_Init_Bounds>`
     - RTBNDI
   * - :doc:`Advanced - Logical Switch for Selection of Slacks <Advanced/CONOPT_Advanced_-_Logical_Switch_Slacks>`
     - LSLACK
   * - :doc:`Advanced - Method for Defined Variables <Advanced/CONOPT_Advanced_-_Method_Defined_Variables>`
     - LMUSDF
   * - :doc:`Advanced - Method for Finding Maximal Step <Advanced/CONOPT_Advanced_-_Method_Finding_Max_Step>`
     - LMMXSF
   * - :doc:`Advanced - Method for Finding Maximal Tight Step <Advanced/CONOPT_Advanced_-_Method_Finding_Max_Tight_Step>`
     - LMMXST
   * - :doc:`Advanced - Method for Linear Feasibility Models <Advanced/CONOPT_Advanced_-_Method_Linear_Feas_Models>`
     - LMETHOD
   * - :doc:`Advanced - Method for Reduced Hessian <Advanced/CONOPT_Advanced_-_Method_Reduced_Hessian>`
     - LMNDIA
   * - :doc:`Advanced - Penalty Constraints Ratio <Advanced/CONOPT_Advanced_-_Penalty_Constraints_Ratio>`
     - RTNOPN
   * - :doc:`Advanced - Relative Objective Accuracy <Advanced/CONOPT_Advanced_-_Relative_Obj_Accuracy>`
     - RTOBJR
   * - :doc:`Advanced - SLP Mode <Advanced/CONOPT_Advanced_-_SLP_Mode>`
     - LSESLP
   * - :doc:`Advanced - SQP Mode <Advanced/CONOPT_Advanced_-_SQP_Mode>`
     - LSESQP
   * - :doc:`Advanced - Steplength Multiplier <Advanced/CONOPT_Advanced_-_Steplength_Multiplier>`
     - RVSTLM
   * - :doc:`Advanced - Use No-Penalty Model <Advanced/CONOPT_Advanced_-_Use_No_Penalty_Model>`
     - DONOPEN
   * - :doc:`Advanced - Zero Filter Tolerance Jacobian Elements <Advanced/CONOPT_Advanced_-_Zero_Filter_Tol_Jacobian_Elem>`
     - RTMINA
   * - :doc:`Debugging - Check 1st Order Derivatives <Debugging/CONOPT_Debugging_-_Check_1st_Order_Der>`
     - LKDEBG
   * - :doc:`Debugging - Check 2nd Order Derivatives <Debugging/CONOPT_Debugging_-_Check_2nd_Order_Der>`
     - LKDEB2
   * - :doc:`Debugging - Tolerance 2nd Order Derivatives Check <Debugging/CONOPT_Debugging_-_Tolerance_2nd_Order_Der_Check>`
     - RT2DRV
   * - :doc:`General - Bound Tolerance <General/CONOPT_General_-_Bound_Tolerance>`
     - RTBND1
   * - :doc:`General - Feasibility Tolerance Triangular Part <General/CONOPT_General_-_Feas_Tol_Triangular>`
     - RTNWTR
   * - :doc:`General - Maximal Feasibility Tolerance <General/CONOPT_General_-_Maximal_Feas_Tol>`
     - RTNWMA
   * - :doc:`General - Method for Initial Basis <General/CONOPT_General_-_Method_Initial_Basis>`
     - LSCRSH
   * - :doc:`General - Minimal Feasibility Tolerance <General/CONOPT_General_-_Minimal_Feas_Tol>`
     - RTNWMI
   * - :doc:`General - Model Is Convex <General/CONOPT_General_-_Model_is_Convex>`
     - ISCONVEX
   * - :doc:`General - Model Is Square System <General/CONOPT_General_-_Model_is_Square>`
     - LSSQRS
   * - :doc:`Limits - Limit on Candidates for Defined Variable <Limits/CONOPT_Limits_-_Limit_Candidates_Defined_Variable>`
     - LFUSDF
   * - :doc:`Limits - Limit on Degenerate Iterations <Limits/CONOPT_Limits_-_Limit_Degenerate_Iterations>`
     - LFDEGI
   * - :doc:`Limits - Limit on Directional 2nd Order Derivative Errors <Limits/CONOPT_Limits_-_Limit_Directional_2nd_Order_Der_Errors>`
     - LF2DRV
   * - :doc:`Limits - Limit on Hessian Evaluation Errors <Limits/CONOPT_Limits_-_Limit_Hessian_Eval_Errors>`
     - LFHSOK
   * - :doc:`Limits - Limit on Linear Feasibility Model Rounds <Limits/CONOPT_Limits_-_Limit_Linear_Feas_Model_Rounds>`
     - NROUNDS
   * - :doc:`Limits - Limit on New Superbasics <Limits/CONOPT_Limits_-_Limit_New_Superbasics>`
     - LFMXNS
   * - :doc:`Limits - Maximal Hessian Dimension <Limits/CONOPT_Limits_-_Maximal_Hessian_Dim>`
     - LFNSUP
   * - :doc:`Limits - Maximum Solution of a Variable <Limits/CONOPT_Limits_-_Maximal_Solution_Variable>`
     - RTMAXV
   * - :doc:`Pivot - Absolute Pivot Tolerance <Pivot/CONOPT_Pivot_-_Absolute_Pivot_Tol>`
     - RTPIVA
   * - :doc:`Pivot - Absolute Pivot Tolerance Initial Basis <Pivot/CONOPT_Pivot_-_Absolute_Pivot_Tol_Initial_Basis>`
     - RTIPVA
   * - :doc:`Pivot - Absolute Pivot Tolerance Nonlinear Elements <Pivot/CONOPT_Pivot_-_Absolute_Pivot_Tol_Nonlinear_Elements>`
     - RTPIVT
   * - :doc:`Pivot - Relative Pivot Tolerance <Pivot/CONOPT_Pivot_-_Relative_Pivot_Tol>`
     - RTPIVR
   * - :doc:`Pivot - Relative Pivot Tolerance during Basis Updates <Pivot/CONOPT_Pivot_-_Relative_Pivot_Tol_during_Basis_Updates>`
     - RTPIVU
   * - :doc:`Pivot - Relative Pivot Tolerance during Ratio Test <Pivot/CONOPT_Pivot_-_Relative_Pivot_Tol_during_Ratio_Test>`
     - RTPIVS
   * - :doc:`Pivot - Relative Pivot Tolerance during Basis Updates <Pivot/CONOPT_Pivot_-_Relative_Pivot_Tol_during_Basis_Updates>`
     - RTIPVR
   * - :doc:`Preprocessing - Preprocessor <Preprocessing/CONOPT_Preprocessing_-_Preprocessor>`
     - DOPREP
   * - :doc:`Preprocessing - Use Interval Evaluations <Preprocessing/CONOPT_Preprocessing_-_Use_Interval_Evaluations>`
     - DOINTV
   * - :doc:`Reporting - Log Frequency <Reporting/CONOPT_Reporting_-_Log_Frequency>`
     - LFILOG
   * - :doc:`Reporting - Log Frequency SLP and SQP <Reporting/CONOPT_Reporting_-_Log_Frequency_SLP_SQP>`
     - LFILOS
   * - :doc:`Scaling - Maximal Scaling Factor <Scaling/CONOPT_Scaling_-_Maximal_Scaling_Factor>`
     - RTMAXS
   * - :doc:`Scaling - Minimal Jacobian Element for Scaling <Scaling/CONOPT_Scaling_-_Minimal_Jacobian_Element_Scaling>`
     - RTMINJ
   * - :doc:`Scaling - Minimal Scaling Factor <Scaling/CONOPT_Scaling_-_Minimal_Scaling_Factor>`
     - RTMINS
   * - :doc:`Scaling - Minimal Scaling Factor 2nd Order Derivatives <Scaling/CONOPT_Scaling_-_Minimal_Scaling_Factor_2nd_Order_Der>`
     - RTMNS2
   * - :doc:`Scaling - Minimal Scaling Tolerance for Variables <Scaling/CONOPT_Scaling_-_Minimal_Scaling_Tol_Vars>`
     - RTMINV
   * - :doc:`Scaling - Rescale Frequency <Scaling/CONOPT_Scaling_-_Rescale_frequency>`
     - LFSCAL
   * - :doc:`Scaling - Scaling Method <Scaling/CONOPT_Scaling_-_Scaling_Method>`
     - LMSCAL
   * - :doc:`Stop Criteria - Accuracy One Dimensional Search <Stop criteria/CONOPT_Stop_Criteria_-_Accuracy_One_Dim_Search>`
     - RTONED
   * - :doc:`Stop Criteria - Limit for Slow Progress <Stop criteria/CONOPT_Stop_Criteria_-_Limit_Slow_Progress>`
     - LFNICR
   * - :doc:`Stop Criteria - Maximal Number of Stalled Iterations <Stop criteria/CONOPT_Stop_Criteria_-_Max_Number_Stalled_Iter>`
     - LFSTAL
   * - :doc:`Stop Criteria - Optimality Tolerance <Stop criteria/CONOPT_Stop_Criteria_-_Optimality_Tol>`
     - RTREDG
   * - :doc:`Stop Criteria - Optimality Tolerance Infeasible <Stop criteria/CONOPT_Stop_Criteria_-_Optimality_Tol_Infeasible>`
     - RTREDI
   * - :doc:`Stop Criteria - Slow Progress Tolerance <Stop criteria/CONOPT_Stop_Criteria_-_Slow_Progress_Tol>`
     - RTOBJL
