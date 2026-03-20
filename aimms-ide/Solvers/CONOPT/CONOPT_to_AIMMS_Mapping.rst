.. _CONOPT_to_AIMMS_Mapping:


CONOPT to AIMMS Mapping
=======================

**Description** 

The table shows in the left column the parameters from CONOPT that can be set in AIMMS; the right column displays for each CONOPT parameter the associated AIMMS option.
	
.. list-table::

   * - **Name in CONOPT**
     - **Option name in AIMMS**
   * - DOINTV
     - :doc:`Preprocessing - Use Interval Evaluations <Preprocessing/CONOPT_Preprocessing_-_Use_Interval_Evaluations>`
   * - DONOPEN
     - :doc:`Advanced - Use No-Penalty Model <Advanced/CONOPT_Advanced_-_Use_No_Penalty_Model>`
   * - DOPREP
     - :doc:`Preprocessing - Preprocessor <Preprocessing/CONOPT_Preprocessing_-_Preprocessor>`
   * - LF2DRV
     - :doc:`Limits - Limit on Directional 2nd Order Derivative Errors <Limits/CONOPT_Limits_-_Limit_Directional_2nd_Order_Der_Errors>`
   * - LFDEGI
     - :doc:`Limits - Limit on Degenerate Iterations <Limits/CONOPT_Limits_-_Limit_Degenerate_Iterations>`
   * - LFHSOK
     - :doc:`Limits - Limit on Hessian Evaluation Errors <Limits/CONOPT_Limits_-_Limit_Hessian_Eval_Errors>`
   * - LFILOG
     - :doc:`Reporting - Log Frequency <Reporting/CONOPT_Reporting_-_Log_Frequency>`
   * - LFILOS
     - :doc:`Reporting - Log Frequency SLP and SQP <Reporting/CONOPT_Reporting_-_Log_Frequency_SLP_SQP>`
   * - LFITER
     - :doc:`Stop Criteria - Iteration Limit <../../Aimms/Options/Solvers General/Stop Criteria/Stop_Criteria_-_Iteration_Limi>`  in 'Solvers - General'
   * - LFMXNS
     - :doc:`Limits - Limit on New Superbasics <Limits/CONOPT_Limits_-_Limit_New_Superbasics>`
   * - LFNICR
     - :doc:`Stop Criteria - Limit for Slow Progress <Stop criteria/CONOPT_Stop_Criteria_-_Limit_Slow_Progress>`
   * - LFNSUP
     - :doc:`Limits - Maximal Hessian Dimension <Limits/CONOPT_Limits_-_Maximal_Hessian_Dim>`
   * - LFSCAL
     - :doc:`Scaling - Rescale Frequency <Scaling/CONOPT_Scaling_-_Rescale_frequency>`
   * - LFSTAL
     - :doc:`Stop Criteria - Maximal Number of Stalled Iterations <Stop criteria/CONOPT_Stop_Criteria_-_Max_Number_Stalled_Iter>`
   * - LFUSDF
     - :doc:`Limits - Limit on Candidates for Defined Variable <Limits/CONOPT_Limits_-_Limit_Candidates_Defined_Variable>`
   * - LKDEB2
     - :doc:`Debugging - Check 2nd Order Derivatives <Debugging/CONOPT_Debugging_-_Check_2nd_Order_Der>`
   * - LKDEBG
     - :doc:`Debugging - Check 1st Order Derivatives <Debugging/CONOPT_Debugging_-_Check_1st_Order_Der>`
   * - LMETHOD
     - :doc:`Advanced - Method for Linear Feasibility Models <Advanced/CONOPT_Advanced_-_Method_Linear_Feas_Models>`
   * - LMMXSF
     - :doc:`Advanced - Method for Finding Maximal Step <Advanced/CONOPT_Advanced_-_Method_Finding_Max_Step>`
   * - LMMXST
     - :doc:`Advanced - Method for Finding Maximal Tight Step <Advanced/CONOPT_Advanced_-_Method_Finding_Max_Tight_Step>`
   * - LMNDIA
     - :doc:`Advanced - Method for Reduced Hessian <Advanced/CONOPT_Advanced_-_Method_Reduced_Hessian>`
   * - LMSCAL
     - :doc:`Scaling - Scaling Method <Scaling/CONOPT_Scaling_-_Scaling_Method>`
   * - LMUSDF
     - :doc:`Advanced - Method for Defined Variables <Advanced/CONOPT_Advanced_-_Method_Defined_Variables>`
   * - LSCRSH
     - :doc:`General - Method for Initial Basis <General/CONOPT_General_-_Method_Initial_Basis>`
   * - LSESLP
     - :doc:`Advanced - SLP Mode <Advanced/CONOPT_Advanced_-_SLP_Mode>`
   * - LSESQP
     - :doc:`Advanced - SQP Mode <Advanced/CONOPT_Advanced_-_SQP_Mode>`
   * - LSLACK
     - :doc:`Advanced - Logical Switch for Selection of Slacks <Advanced/CONOPT_Advanced_-_Logical_Switch_Slacks>`
   * - LSSQRS
     - :doc:`General - Model Is Square System <General/CONOPT_General_-_Model_is_Square>`
   * - ISCONVEX
     - :doc:`General - Model Is Convex <General/CONOPT_General_-_Model_is_Convex>`
   * - NROUNDS
     - :doc:`Limits - Limit on Linear Feasibility Model Rounds <Limits/CONOPT_Limits_-_Limit_Linear_Feas_Model_Rounds>`
   * - RT2DRV
     - :doc:`Debugging - Tolerance 2nd Order Derivatives Check <Debugging/CONOPT_Debugging_-_Tolerance_2nd_Order_Der_Check>`
   * - RTBND1
     - :doc:`General - Bound Tolerance <General/CONOPT_General_-_Bound_Tolerance>`
   * - RTBNDI
     - :doc:`Advanced - Fixed Variables Tolerance Initial Bounds <Advanced/CONOPT_Advanced_-_Fixed_Var_Tol_Init_Bounds>`
   * - RTBNDT
     - :doc:`Advanced - Fixed Variables Tolerance Derived Bounds <Advanced/CONOPT_Advanced_-_Fixed_Var_Tol_Derived_Bounds>`
   * - RTBOX
     - :doc:`Advanced - Box Size Tolerance <Advanced/CONOPT_Advanced_-_Box_Size_Tolerance>`
   * - RTBOXF
     - :doc:`Advanced - Box Size Factor Linear Variables <Advanced/CONOPT_Advanced_-_Box_Size_Factor_Linear_Var>`
   * - RTBOXL
     - :doc:`Advanced - Box Size Tolerance Linear <Advanced/CONOPT_Advanced_-_Box_Size_Tolerance_Linear>`
   * - RTIPVA
     - :doc:`Pivot - Absolute Pivot Tolerance Initial Basis <Pivot/CONOPT_Pivot_-_Absolute_Pivot_Tol_Initial_Basis>`
   * - RTIPVR
     - :doc:`Pivot - Relative Pivot Tolerance Initial Basis <Pivot/CONOPT_Pivot_-_Relative_Pivot_Tol_Initial_Basis>`
   * - RTMAXS
     - :doc:`Scaling - Maximal Scaling Factor <Scaling/CONOPT_Scaling_-_Maximal_Scaling_Factor>`
   * - RTMAXV
     - :doc:`Limits - Maximum Solution of a Variable <Limits/CONOPT_Limits_-_Maximal_Solution_Variable>`
   * - RTMINA
     - :doc:`Advanced - Zero Filter Tolerance Jacobian Elements <Advanced/CONOPT_Advanced_-_Zero_Filter_Tol_Jacobian_Elem>`
   * - RTMINJ
     - :doc:`Scaling - Minimal Jacobian Element for Scaling <Scaling/CONOPT_Scaling_-_Minimal_Jacobian_Element_Scaling>`
   * - RTMINS
     - :doc:`Scaling - Minimal Scaling Factor <Scaling/CONOPT_Scaling_-_Minimal_Scaling_Factor>`
   * - RTMINV
     - :doc:`Scaling - Minimal Scaling Tolerance for Variables <Scaling/CONOPT_Scaling_-_Minimal_Scaling_Tol_Vars>`
   * - RTMNS2
     - :doc:`Scaling - Minimal Scaling Factor 2nd Order Derivatives <Scaling/CONOPT_Scaling_-_Minimal_Scaling_Factor_2nd_Order_Der>`
   * - RTNOPN
     - :doc:`Advanced - Penalty Constraints Ratio <Advanced/CONOPT_Advanced_-_Penalty_Constraints_Ratio>`
   * - RTNWMA
     - :doc:`General - Maximal Feasibility Tolerance <General/CONOPT_General_-_Maximal_Feas_Tol>`
   * - RTNWMI
     - :doc:`General - Minimal Feasibility Tolerance <General/CONOPT_General_-_Minimal_Feas_Tol>`
   * - RTNWTR
     - :doc:`General - Feasibility Tolerance Triangular Part <General/CONOPT_General_-_Feas_Tol_Triangular>`
   * - RTOBJL
     - :doc:`Stop Criteria - Slow Progress Tolerance <Stop criteria/CONOPT_Stop_Criteria_-_Slow_Progress_Tol>`
   * - RTOBJR
     - :doc:`Advanced - Relative Objective Accuracy <Advanced/CONOPT_Advanced_-_Relative_Obj_Accuracy>`
   * - RTONED
     - :doc:`Stop Criteria - Accuracy One Dimensional Search <Stop criteria/CONOPT_Stop_Criteria_-_Accuracy_One_Dim_Search>`
   * - RTPIVA
     - :doc:`Pivot - Absolute Pivot Tolerance <Pivot/CONOPT_Pivot_-_Absolute_Pivot_Tol>`
   * - RTPIVR
     - :doc:`Pivot - Relative Pivot Tolerance <Pivot/CONOPT_Pivot_-_Relative_Pivot_Tol>`
   * - RTPIVS
     - :doc:`Pivot - Relative Pivot Tolerance during Ratio Test <Pivot/CONOPT_Pivot_-_Relative_Pivot_Tol_during_Ratio_Test>`
   * - RTPIVT
     - :doc:`Pivot - Absolute Pivot Tolerance Nonlinear Elements <Pivot/CONOPT_Pivot_-_Absolute_Pivot_Tol_Nonlinear_Elements>`
   * - RTPIVU
     - :doc:`Pivot - Relative Pivot Tolerance during Basis Updates <Pivot/CONOPT_Pivot_-_Relative_Pivot_Tol_during_Basis_Updates>`
   * - RTREDG
     - :doc:`Stop Criteria - Optimality Tolerance <Stop criteria/CONOPT_Stop_Criteria_-_Optimality_Tol>`
   * - RTREDI
     - :doc:`Stop Criteria - Optimality Tolerance Infeasible <Stop criteria/CONOPT_Stop_Criteria_-_Optimality_Tol_Infeasible>`
   * - RVSTLM
     - :doc:`Advanced - Steplength Multiplier <Advanced/CONOPT_Advanced_-_Steplength_Multiplier>`
   * - RVTIME
     - :doc:`Stop Criteria - Time Limit <../../Aimms/Options/Solvers General/Stop Criteria/Stop_Criteria_-_Time_Limit>`  in 'Solvers - General'
