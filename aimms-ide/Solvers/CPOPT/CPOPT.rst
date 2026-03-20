.. _SolverCPOPT:


CP Optimizer
=================

**Description** 

IBM ILOG CP Optimizer (CPOPT for short) is a software package for constraint programming targeting both constraint satisfaction problems and optimization problems. It contains powerful methods for finding feasible solutions and improving them. The strength of CP Optimizer is that it removes the need for you to write and maintain a search strategy.



CP Optimizer is equipped with parameters that influence the performance of CP Optimizer. AIMMS is equipped with options that set the parameters in CP Optimizer. Options in AIMMS can be set in the options dialog box.



Note that the general solvers options **MIP Absolute Optimality Tolerance**  and **MIP Relative Optimality Tolerance**  are not used by CP Optimizer. You should use the CP Optimizer options **Optimality Tolerance**  and **Relative Optimality Tolerance**  instead. Also the general solvers option **Maximal Number of Integer Solutions**  is not used by CP Optimizer; you should use CP Optimizer option **Solution Limit**  instead.



**Best Bound** 

CP Optimizer now maintains a bound on the objective (a lower bound for minimization problems and an upper bound for maximization problems). This bound is displayed in the Progress Window when a new bound is found, along with the optimality gap when an improving solution has been found. At the end of the search, the best bound and gap are displayed.



**Learn more about** 

*	`CP Optimizer <https://www.ibm.com/products/ilog-cplex-optimization-studio/cplex-cp-optimizer>`_ (Internet link)
*	:doc:`CPOPT_to_AIMMS_Mapping`  
*	:doc:`AIMMS_to_CPOPT_Mapping`  
*	:doc:`../../Aimms/Options/AIMMS_Execution_Options`  
*	:doc:`../../Aimms/Options/Solvers General/MIP Options/MIP_Options_-_Maximal_Number_o`  
*	:doc:`../../Aimms/Options/Solvers General/MIP Options/MIP_Options_-_MIP_Absolute_Opt`  
*	:doc:`../../Aimms/Options/Solvers General/MIP Options/MIP_Options_-_MIP_Relative_Opt`  
*	:doc:`General/CPOPT_General_-_Optimality_tolerance` 
*	:doc:`General/CPOPT_General_-_Relative_optimality_tolerance` 
*	:doc:`General/CPOPT_General_-_Solution_limit` 
