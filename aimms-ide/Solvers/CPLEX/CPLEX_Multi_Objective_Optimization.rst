.. _CPLEX_Multi_Objective_Optimization:

Multi-Objective Optimization
============================

CPLEX allows you to define a mixture of blended and lexicographic (or hierarchical) objectives.

A blended objective consists of the linear combination of several objectives with given weights.

A lexicographic objective assumes that the objectives can be ranked in order of importance. A solution is considered
lexicographically better than another solution if it is better in the first objective where they differ (following
the order). For a minimization problem, an optimal solution is one that is lexicographically minimal.

A variable can be specified as a multi-objective variable by using the AIMMS routine :any:`GMP::Column::SetAsMultiObjective`.
For example, to mark the variables TotalDist and TotalTime in a mathematical program 'MP' as multi-objective variables
and solve the math program use


.. code-block:: aimms

    gmpMP := GMP::Instance::Generate( MP );

    GMP::Column::SetAsMultiObjective( gmpMP, TotalDist, 2, 1.0, 0, 0.1 );
    GMP::Column::SetAsMultiObjective( gmpMP, TotalTime, 1, 1.0, 0, 0.0 );

    GMP::Instance::Solve( gmpMP );


where 'gmpMP' is an element parameter with range :aimms:set:`AllGeneratedMathematicalPrograms`.


AIMMS will not actually pass the multi-objective variables to CPLEX but instead substitute these variables by the linear
expression that defines them. For example, if TotalDist is defined as 10*x1 + 20*x2 then CPLEX will receive 10*x1 + 20*x2
as the first multi-objective.


**Priorities and weights** 

The CPLEX multi-objective optimization algorithm sorts the objectives by decreasing priority value. If several objectives
have the same priority, they are blended in a single objective using the weight attributes provided. As a result, CPLEX
constructs a sorted list of objectives (or blended objectives), each with a unique priority. CPLEX can then proceed to
find the lexicographically minimal (or maximal) solution for this order.


To obtain this solution, each objective is optimized in turn by decreasing order of the priority value in a hierarchical manner.
Whenever the optimal solution for an objective (or blended objective) is found, CPLEX imposes that, for the remaining (lower
priority) objectives, the only solutions considered are those that are also optimal for the previously (higher priority) optimized
objectives.


The priority of each objective can be specified using the third argument of the routine GMP::Column::SetAsMultiObjective. Its fourth
argument defines the weight by which the objective coefficients are multiplied when forming a blended objective, i.e., if multiple
objectives have the same priority. In the example above in which TotalDist is defined as 10*x1 + 20*x2 the objective coefficients
are 10 and 20 (for x1 and x2 respectively).


**Absolute and relative tolerance** 

The last two arguments of the routine :any:`GMP::Column::SetAsMultiObjective` specify the absolute and relative tolerance respectively.
They can be used to relax the requirement that in each step the objective is optimized among the solutions that are optimal to the
previous optimization problems. More precisely, for each objective, the absolute and relative tolerance specify, in absolute and
relative terms, the maximum deviations allowed from the optimal value of that objective. However, the meaning of the relaxation of
the objective depends on whether the multi-objective problem is an LP or MIP.


**MIP:** 

The relative or absolute deviation is incorporated into a constraint on the associated objective. Leaving these values at their
defaults of 0 implies restricting the next optimization to only consider solutions from the optimal set from the previous optimization.
In the above example, CPLEX will first optimize the math program using TotalDist as the (single) objective (because it has the highest
priority). Next CPLEX will use TotalTime as the (single) objective and it will consider all solutions for which TotalDist is inside 10%
of the optimal value of TotalDist; this is specified by the 0.1 value for the relative tolerance in the first
:any:`GMP::Column::SetAsMultiObjective` call.


**LP:** 

For LPs, CPLEX uses a typically faster method involving reduced cost fixing to enforce lexicographic multi-objective optimization.
This alters the meaning of the absolute and relative tolerances. The absolute tolerance defines the threshold for reduced costs above
which non-basic variables in the associated LP solve will be fixed at the bound at which they reside. This typically will be a relatively
small value like the optimality tolerance (whose default is 1e-6). It is used to define a meaningful value that defines a significant
reduced cost in the context of the multi-objective model (in contrast to the meaningful reduced cost defined by the optimality tolerance,
which is for a single LP solve). Given this interpretation, the relative tolerance has no meaningful definition and is not used. **Note**:
If you want the MIP behavior, where the deviation is controlled more directly, you can add a dummy binary variable to the model, thereby
transforming it into a MIP.


**Optimization direction** 

CPLEX only allows you to specify one optimization direction for the whole set of multi-objectives (minimization or maximization). However,
by specifying a negative weight for an objective, one can reverse the optimization direction of any objective.


**Using different option settings** 

During the solution process, you may prefer that optimization problems with different priorities are solved with different option settings.
CPLEX makes this possible by using parameter files, which can be activated with the option **Read Parameter File**. This way you can specify
different settings for the MIP relative optimality tolerance or the time limit for each optimization pass.


**Note** 

*	Multi-objective optimization is not supported for models with quadratic terms in the objectives or in the constraints.
*	Sensitivity information and basis information are not available for multi-objective optimization.
*	Solution polishing is not available for multi-objective optimization.
*	The branch, candidate, cut, heuristic and lazy constraints callback procedures are not supported for multi-objective optimization. (The incumbent callback is supported for multi-objective optimization; see the section :ref:`CPLEX_Threads_search_strat_and_callb` .)
*	Generic callbacks will be used for solving multi-objective optimization models even if the option **Use Generic Callbacks**  is set to 'No'. As a consequence, when solving a multi-objective LP model CPLEX cannot be interrupted and no progress information is provided during the solve.


**Learn more about** 

*	:any:`GMP::Column::SetAsMultiObjective`
*	:ref:`CPLEX_Threads_search_strat_and_callb` 
*	:ref:`option-CPLEX-read_parameter_file` 
*	:ref:`option-CPLEX-use_generic_callbacks` 

