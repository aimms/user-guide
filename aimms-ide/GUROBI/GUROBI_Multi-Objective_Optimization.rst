.. _GUROBI_Multi-Objective_Optimization:


Multi-Objective Optimization
============================

Gurobi 12.0 allows you to define a mixture of blended and lexicographic (or hierarchical) objectives.



A blended objective consists of the linear combination of several objectives with given weights.



A lexicographic objective assumes that the objectives can be ranked in order of importance. A solution is considered lexicographically better than another solution if it is better in the first objective where they differ (following the order). For a minimization problem, an optimal solution is one that is lexicographically minimal.



A variable can be specified as a multi-objective variable by using the AIMMS routine GMP::Column::SetAsMultiObjective. For example, to mark the variables TotalDist and TotalTime in a mathematical program 'MP' as multi-objective variables and solve the math program use



	gmpMP := GMP::Instance::Generate( MP );

    

	GMP::Column::SetAsMultiObjective( gmpMP, TotalDist, 2, 1.0, 0, 0.1 );

	GMP::Column::SetAsMultiObjective( gmpMP, TotalTime, 1, 1.0, 0, 0.0 );



	GMP::Instance::Solve( gmpMP );



where 'gmpMP' is an element parameter with range 'AllGeneratedMathematicalPrograms'.



AIMMS will not actually pass the multi-objective variables to Gurobi but instead substitute these variables by the linear expression that defines them. For example, if TotalDist is defined as 10*x1 + 20*x2 then Gurobi will receive 10*x1 + 20*x2 as the first multi-objective.



**Priorities and weights** 

The Gurobi multi-objective optimization algorithm sorts the objectives by decreasing priority value. If several objectives have the same priority, they are blended in a single objective using the weight attributes provided. As a result, Gurobi constructs a sorted list of objectives (or blended objectives), each with a unique priority. Gurobi can then proceed to find the lexicographically minimal (or maximal) solution for this order.



To obtain this solution, each objective is optimized in turn by decreasing order of the priority value in a hierarchical manner. Whenever the optimal solution for an objective (or blended objective) is found, Gurobi imposes that, for the remaining (lower priority) objectives, the only solutions considered are those that are also optimal for the previously (higher priority) optimized objectives.



The priority of each objective can be specified using the third argument of the routine GMP::Column::SetAsMultiObjective. Its fourth argument defines the weight by which the objective coefficients are multiplied when forming a blended objective, i.e., if multiple objectives have the same priority. In the example above in which TotalDist is defined as 10*x1 + 20*x2 the objective coefficients are 10 and 20 (for x1 and x2 respectively).



**Absolute and relative tolerance** 

The last two arguments of the routine GMP::Column::SetAsMultiObjective specify the absolute and relative tolerance respectively. They can be used to relax the requirement that in each step the objective is optimized among the solutions that are optimal to the previous optimization problems. More precisely, for each objective, the absolute and relative tolerance specify, in absolute and relative terms, the maximum deviations allowed from the optimal value of that objective. However, the meaning of the relaxation of the objective depends on whether the multi-objective problem is an LP or MIP.



**MIP:** 

By default, the hierarchical approach won’t allow later objectives to degrade earlier objectives. This behavior can be relaxed for MIPs through a pair of tolerances: a relative and an absolute tolerance. By setting one of these for a particular objective, you can indicate that later objectives are allowed to degrade this objective by the specified relative or absolute amount, respectively. In our example, if the optimal value for the first objective is 100, and if we set the absolute tolerance for this objective to 20, then the second optimization step would find the best solution for the second objective from among all solutions with objective 120 or better for the first objective. Note that if you modify both tolerances, later optimizations would use the looser of the two values (i.e., the one that allows the larger degradation).



**LP:** 

Objective degradations are handled differently for multi-objective LP models. For LP models, solution quality for higher-priority objectives is maintained by fixing some variables to their values in previous optimal solutions. These fixings are decided using variable reduced costs. The absolute tolerance indicates the amount by which a fixed variable’s reduced cost is allowed to violate dual feasibility, whereas the relative tolerance is simply ignored. **Note** : If you want the MIP behavior, where the degradation is controlled more directly, you can add a dummy binary variable to the model, thus transforming it into a MIP. Solving the resulting multi-objective MIP can be much more time consuming than solving the original multi-objective LP.



**Optimization direction** 

Gurobi only allows you to specify one optimization direction for the whole set of multi-objectives (minimization or maximization). However, by specifying a negative weight for an objective, one can reverse the optimization direction of any objective.



**Using different option settings** 

During the solution process, you may prefer that optimization problems with different priorities are solved with different option settings. Gurobi makes this possible by using parameter files, which can be activated with the option **Read Parameter File** . This way you can specify different settings for the MIP relative optimality tolerance or the time limit for each optimization pass.



**Note** 

*	Multi-objective optimization is not supported for models with quadratic terms in the objectives or in the constraints.
*	Sensitivity information and basis information are not available for multi-objective optimization.




**Learn more about** 

*	Search for GMP::Column::SetAsMultiObjective (Function Reference)
*	:ref:`GUROBI_General_-_Multi_objective_method` 
*	:ref:`GUROBI_Presolve_-_Multi_Objective_Presolve` 
*	:ref:`GUROBI_General_-_Read_Parameter_File` 



