.. _option-CPLEX-display_solution_statistics:


Display Solution Statistics
===========================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Automatic	



This option can be used to display statistics that give information about the quality of the solution. Possible values are:



*	Automatic
*	Off
*	On




If the value of this option equals 'On' then AIMMS will display information related to the quality of the solution, depending on the model type and the algorithm (simplex or barrier) that was used. If the value of this option equals 'Automatic' then AIMMS will display this information only if the value of the option **Check Solution**  equals 'Yes'.





The information is printed in the AIMMS Message Window. It is also printed in the CPLEX status file if the general solvers option **Solver Listing Messages**  is set to 'All' or 'Remark'. The CPLEX status file is named 'CPLEX 22.1.sta' and it is placed in the log directory of the AIMMS project.





For LP and QP problems that are solved using the simplex algorithm (or the sifting algorithm), the following statistics, both scaled and unscaled, are printed:





#.  :ref:`option-CPLEX-display_solution_statistics` ;
#.  :ref:`option-CPLEX-display_solution_statistics` ;
#.  :ref:`option-CPLEX-display_solution_statistics` ;
#.  :ref:`option-CPLEX-display_solution_statistics` ;
#.  :ref:`option-CPLEX-display_solution_statistics` ;
#.  :ref:`option-CPLEX-display_solution_statistics` ;
#.  :ref:`option-CPLEX-display_solution_statistics` ;
#.  :ref:`option-CPLEX-display_solution_statistics` ;
#.  :ref:`option-CPLEX-display_solution_statistics`  (unscaled only).




Note: The basis condition number will not be calculated it the option **Memory Emphasis**  is switched on.





For LP and QP problems that are solved using the barrier algorithm, the following statistics are printed:





#.  :ref:`option-CPLEX-display_solution_statistics` ;
#.  :ref:`option-CPLEX-display_solution_statistics` ;
#.  :ref:`option-CPLEX-display_solution_statistics` ;
#.  :ref:`option-CPLEX-display_solution_statistics` ;
#.  :ref:`option-CPLEX-display_solution_statistics` ;
#.  :ref:`option-CPLEX-display_solution_statistics` ;
#.  :ref:`option-CPLEX-display_solution_statistics` ;
#.  :ref:`option-CPLEX-display_solution_statistics` .




For MIP and MIQP problems the following statistics are printed:





#.  :ref:`option-CPLEX-display_solution_statistics` ;
#.  :ref:`option-CPLEX-display_solution_statistics` ;
#.  :ref:`option-CPLEX-display_solution_statistics` ;
#.  :ref:`option-CPLEX-display_solution_statistics` ;
#.  :ref:`option-CPLEX-display_solution_statistics` ;
#.  :ref:`option-CPLEX-display_solution_statistics`  (if indicator constraints are present).




Note: Statistic nr. 5 reports bound violations of slack variables. A bound violation of a slack variable implies an infeasibility in the corresponding constraint.





For QCP and MIQCP problems the following statistics are printed:





#.  :ref:`option-CPLEX-display_solution_statistics` ;
#.  :ref:`option-CPLEX-display_solution_statistics` ;
#.  :ref:`option-CPLEX-display_solution_statistics` ;
#.  :ref:`option-CPLEX-display_solution_statistics` ;
#.  :ref:`option-CPLEX-display_solution_statistics`  (only MIQCP);
#.  :ref:`option-CPLEX-display_solution_statistics` ;
#.  :ref:`option-CPLEX-display_solution_statistics` ;
#.  :ref:`option-CPLEX-display_solution_statistics`  (if indicator constraints are present).




Note: Statistic nr. 6 reports bound violations of slack variables. A bound violation of a slack variable implies an infeasibility in the corresponding constraint.





Below the statistics are discussed in more detail.








**Bound Infeasibility: Identifying Largest Bound Violation** 





The maximum bound infeasibility identifies the largest bound violation. This information may help you discover the cause of infeasibility in your problem. If the largest bound violation exceeds the feasibility tolerance of your problem by only a small amount, then you may be able to get a feasible solution to the problem by increasing the option **Feasibility**  for feasibility tolerance. Its range is between 1e-9 and 0.1. Its default value is 1e-6. 





**Reduced-Cost Infeasibility** 





The maximum reduced-cost infeasibility identifies a value for the optimality tolerance that would cause CPLEX to perform additional iterations. It refers to the infeasibility in the dual slack associated with reduced costs. Whether CPLEX terminated with an optimal or infeasible solution, if the maximum reduced-cost infeasibility is only slightly smaller in absolute value than the optimality tolerance, then solving the problem with a smaller optimality tolerance may result in an improvement in the objective function. 





To change the optimality tolerance, set the option **Optimality** . 





**Constraint Residual / Slack Bound Violation** 





The maximum constraint residual identifies the maximum constraint violation. CPLEX simplex optimizers control these residuals only indirectly by applying numerically sound methods to solve the given linear system. When CPLEX terminates with an infeasible solution, all infeasibilities will appear as bound violations on structural or slack variables, not constraint violations. The maximum constraint residual may help you decide whether a model of your problem is poorly scaled, or whether the final basis (whether it is optimal or infeasible) is ill-conditioned.





Normally CPLEX reports infeasibilities in the constraints as bound violations of the corresponding slack variables.





**Dual Residual** 





The maximum dual residual indicates the numeric accuracy of the reduced costs in the current solution. By construction, in exact arithmetic, the dual residual of a basic solution is always 0 (zero). A nonzero value is thus the effect of round-off error due to finite-precision arithmetic in the computation of the dual solution vector. Thus, a significant nonzero value indicates ill conditioning. 





**Absolute Variable Values: Detecting Ill-Conditioned Problems** 





When you are trying to decide whether your problem is ill-conditioned, you also need to consider the following absolute values:





*   variables;
*   slack variables;
*   dual variables;
*   reduced costs (i.e., dual slack variables).




If one of these values is very large (above 1e6) then this is an indication that the model might be numerical instable.





**Basis Condition Number** 





The basis condition number ('Kappa') can be used to measure the sensitivity of a linear problem to the problem data. You might also think of the basis condition number as the number of places in precision that can be lost.





For example, if the basis condition number at optimality is 1e+13, then a change in a single matrix coefficient in the thirteenth place (counting from the right) may dramatically alter the solution. Furthermore, since many computers provide about 16 places of accuracy in double precision, only three accurate places are left in such a solution. Even if an answer is obtained, perhaps only the first three significant digits are reliable.





**Integer Infeasibility** 





The integer infeasibility measures the difference between the solution value of an integer variable and the nearest integer value. Ideally this difference is 0, however by default a small deviation is allowed, as controlled by the option **Integrality** . The range of this option is between 0.0 and 0.5. Its default value is 1e-5.





**Duality Gap** 





The duality gap measures the difference between the primal and dual objective.





**Complementarity** 





The CPLEX barrier optimizer stops when it finds feasible primal and dual solutions that are complementary, within some tolerance. This tolerance is controlled by the option **Barrier Convergence Tolerance** .





**Note** 

*	This option will only be effective if a solution is found by CPLEX.
*	For LP problems, if the barrier algorithm is used with a crossover step, as controlled by the option **Solution Type** , then information will be displayed related to the quality of the simplex solution.
*	The solution statistics are displayed before the postsolve step is executed (if any; as controlled by the general solvers option **Postsolve** ).
*	For MIP problems, the option **MIP Kappa**  offers a way to calculate the condition number.
*	The solution statistics will not be displayed for models with multiple objectives.




**Learn more about** 

*	:ref:`option-CPLEX-barrier_convergence_tolerance`  
*	:ref:`option-CPLEX-check_solution`  
*	:ref:`option-CPLEX-feasibility`  
*	:ref:`option-CPLEX-integrality`  
*	:ref:`option-CPLEX-lp_method`  
*	:ref:`option-CPLEX-memory_emphasis`  
*	:ref:`option-CPLEX-mip_kappa`  
*	:ref:`option-CPLEX-optimality`  
*	:ref:`option-AIMMS-postsolve` 
*	:ref:`option-CPLEX-solution_type`  
*	:ref:`option-AIMMS-solver_listing_messages`  
