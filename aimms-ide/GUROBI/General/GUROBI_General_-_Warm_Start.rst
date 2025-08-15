.. _GUROBI_General_-_Warm_Start:


Warm Start
==========



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Original problem	



This option controls whether and how Gurobi uses warm start information for an LP optimization. Possible values are:



*	Off
*	Original problem
*	Presolved problem




The setting of 'Presolved problem' is particularly useful for communicating advanced start information while retaining the performance benefits of presolve. A warm start can consist of any combination of basis statuses, a primal start vector, or a dual start vector.





As a general rule, switching off this option ignores any start information and solves the model from scratch. Setting it to 'Original problem' (the default) uses the provided warm start information to solve the original, unpresolved problem, regardless of whether presolve is enabled. Setting it to 'Presolved problem' uses the start information to solve the presolved problem, assuming that presolve is enabled. This involves mapping the solution of the original problem into an equivalent (or sometimes nearly equivalent) crushed solution of the presolved problem. If presolve is disabled, then setting 'Presolved problem' still prioritizes start vectors, while setting 'Original problem' prioritizes basis statuses. Taken together, this option setting, the LP algorithm specified by the **Method**  option, and the available advanced start information determine whether Gurobi will use basis statuses only, basis statuses augmented with information from start vectors, or a basis obtained by applying the crossover method to the provided primal and dual start vectors to jump start the optimization.





When the **Method**  option requests the barrier solver, primal and dual start vectors are prioritized over basis statuses (but only if you provide both). These start vectors are fed to the crossover procedure. This is the same crossover that is used to compute a basic solution from the interior solution produced by the core barrier algorithm, but in this case crossover is started from arbitrary start vectors. If you set this option to 'Original problem', crossover will be invoked on the original model using the provided vectors. Any provided basis information will not be used in this case. If you set this option to 'Presolved problem', crossover will be invoked on the presolved model using crushed start vectors. If you set this option to 'Presolved problem' and provide a basis but no start vectors, the basis will be used to compute the corresponding primal and dual solutions on the original model. Those solutions will then be crushed and used as primal and dual start vectors for the crossover, which will then construct a basis for the presolved model. Note that for all of these settings and start combinations, no barrier algorithm iterations are performed.





The simplex algorithms provide more warm-starting options. With setting 'Original problem', simplex will start from a provided basis, if available. Otherwise, it uses a provided start vector to refine the crash basis it computes. Primal simplex will use a primal start vector and dual simplex will use a dual start vector in this refinement process.





With a value of 'Presolved problem', simplex will use the crushed start vector on the presolved model (primal start vector for primal simplex, dual start vector for dual) to refine the crash basis. This is true regardless of whether the start is derived from start vectors or a starting basis from the original model. The difference is that if you provide an advanced basis, the basis will be used to compute the corresponding primal and dual solutions on the original model from which the primal or dual start on the presolved model will be derived.





**Note** 

*	This option only affects linear programming (LP) models.




**Learn more about** 

*	:ref:`GUROBI_General_-_Method` 
