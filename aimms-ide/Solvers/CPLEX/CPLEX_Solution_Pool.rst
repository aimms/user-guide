.. _CPLEX_Solution_Pool:


Solution Pool
=============

The solution pool stores multiple solutions to a mixed integer programming (MIP) model. With this feature, you can direct the algorithm to generate multiple solutions in addition to the optimal solution. For example, some constraints may be difficult to formulate efficiently as linear expressions, or the objective may be difficult to quantify exactly. In such cases, obtaining multiple solutions will help you choose one which best fits all your criteria, including the criteria that could not be expressed easily in a conventional MIP model.



Furthermore, you can use the solution pool and tools associated with it to explore and evaluate alternative solutions in a variety of these:


*   You can collect solutions within a given percentage of the optimal solution. To do so, apply the solution pool gap options **Pool Absolute Objective Gap**  or **Pool Relative Objective Gap** .


*   You can collect a set of diverse solutions. To do so, use the option **Pool Replacement Strategy**  to set the solution pool replacement strategy to 'Diverse solutions'. In order to control the diversity of solutions even more finely, you can apply a diversity filter, as explained in :ref:`CPLEX_Filters`.
*   In an advanced application of the populate feature, you can collect solutions with specific properties by using filters. Filters allow you to control properties of the solutions generated and stored in the solution pool. See :ref:`CPLEX_Filters`.
*   You can collect all solutions or all optimal solutions to a MIP model. To do so, set the option **Pool Intensity**  to 'Very aggressive'.



The populate algorithm used to populate the solution pool is always preceded by a MIP optimization (the first phase) in which the problem is solved to optimality (or some stopping criterion set by the user) while it sets up a branch and cut tree for the second phase. Next, in the second phase, the populate algorithm generates multiple solutions by using the information computed and stored in the first phase and by continuing to explore the tree.



**Invoking the solution pool** 

The option **Do Populate**  should be switched on before a normal solve statement (or before GMP::Instance::Solve) to let CPLEX fill the solution pool.



The amount of preparation in the first phase and the intensity of exploration in the second phase are controlled by the solution pool intensity option **Pool Intensity** .

Optimality is not a stopping criterion for the populate algorithm. Even if the optimality gap is zero, this routine will still try to find alternative solutions. The stopping criteria for the populate algorithm are these:


*   The option **Population Limit**  controls how many solutions are generated before stopping. Its default value is 20. 
*   The time limit, controlled by the general solvers option **Time Limit** , as in standard MIP optimization.
*   The populate time limit for the second phase, controlled by the option **Populate Time Limit** .
*   The node limit, controlled by the option **Maximal Number of Nodes** , as in standard MIP optimization. 
*   In the absence of other stopping criteria, the populate algorithm stops when it cannot enumerate any more solutions. In particular, if the user specifies an objective tolerance with the relative or absolute solution pool gap options, **Pool Relative Objective Gap**  and **Pool Absolute Objective Gap**  respectively, the populate algorithm stops if it cannot enumerate any more solutions within the specified objective tolerance. There may exist additional solutions that satisfy the specified objective tolerance; depending on the solution pool intensity option, the populate algorithm may or may not enumerate all of them; according to certain settings of the solution pool intensity option, the populate algorithm may stop when it has enumerated a subset of additional solutions satisfying the specified objective tolerance. 



The populate algorithm does not try to generate multiple solutions for unbounded MIP problems. As soon as the proof of unboundedness is obtained, the populate algorithm stops.



**Accessing a solution in the solution pool** 

All solutions in the solution pool will be stored in the solution repository of the mathematical program. At position 1 of that solution repository the incumbent solution is stored, at position 2 the solution with the second best objective value, and so on. The incumbent solution at position 1 might not satisfy the filters (if any); all other solutions in the solution repository will satisfy the filters. Solutions in the solution repository can be send to the model identifiers by using the AIMMS routine GMP::Solution::SendToModel. For example, with



	GMP::Solution::SendToModel( 'frac1', 2 );



the second best solution for the mathematical program 'frac1' will be send to the model identifiers.



**Learn more about** 

*	:ref:`option-CPLEX-do_populate`  
*	:ref:`CPLEX_Filters` 
*	:ref:`option-CPLEX-maximal_number_of_nodes`  
*	:ref:`option-CPLEX-pool_absolute_objective_gap`  
*	:ref:`option-CPLEX-pool_intensity`  
*	:ref:`option-CPLEX-pool_relative_objective_gap`  
*	:ref:`option-CPLEX-pool_replacement_strategy`  
*	:ref:`option-CPLEX-populate_time_limit`  
*	:ref:`option-CPLEX-population_limit`  
*	:ref:`option-AIMMS-time_limit`  
*	:any:`GMP::Solution::SendToModel`
