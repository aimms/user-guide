
ODH CPLEX
==========

**Description** 

ODH-CPLEX is a tool for solving, first of all, mixed integer linear optimization problems. Such problems are conventionally written like this:

.. math::

   \begin{aligned}
   & \text{Minimize:} \quad && c_{1}x_{1} + c_{2}x_{2} + \ldots + c_{n}x_{n} \\
   & \text{Subject to:} \\
   & && a_{11}x_{1} + a_{12}x_{2} + \ldots + a_{1n}x_{n} \sim b_1 \\
   & && a_{21}x_{1} + a_{22}x_{2} + \ldots + a_{2n}x_{n} \sim b_2 \\
   & && \vdots \\
   & && a_{m1}x_{1} + a_{m2}x_{2} + \ldots + a_{mn}x_{n} \sim b_m \\
   & && l_1 \leq x_1 \leq u_1 \\
   & && \vdots \\
   & && l_n \leq x_n \leq u_n
   \end{aligned}

where,

* :math:`x` is the vector of variables,
* :math:`a`, :math:`b`, and :math:`c` are real numbers,
* :math:`l` and :math:`u` are vectors of lower and upper bounds, and
* :math:`\sim` can be either <=, >=, or =.

Some of the lower bounds may be :math:`-\infty` and some of the upper bounds may be :math:`\infty`.
The scalar value :math:`n` will denote the number of variables and :math:`m` the number of equations.

The optimization problem can be maximized instead of minimized.

ODH-CPLEX requires that some of the variables are binary or integer. These problems are known as mixed integer programs or MIPs. ODH-CPLEX can also handle certain problems in which the objective function is not linear but quadratic. Such problems are called mixed integer quadratic programs (MIQP) if all constraints are linear. ODH-CPLEX can also handle certain problems in which some of the constraints are quadratic, while the objective function is linear or quadratic. These problems are called mixed integer quadratically constrained programs (MIQCP). ODH-CPLEX can also be used for some types of second-order cone constraints.



**Heuristic Methods** 

ODH-CPLEX is a set of heuristic methods for finding feasible solutions to Mixed Integer Programming (MIP) models that uses IBM CPLEX as its underlying solver engine. It is designed for large-scale models which a MIP solver would find intractable: either by it being unable to find feasible solutions at all or; more usually, by being unable to find feasible solutions of adequate quality in the time available to its user.



ODH-CPLEX is intended for users who are familiar with MIP modelling and have some knowledge of using the IBM CPLEX commercial MIP software. ODH-CPLEX does not demand expert specialism in this field. 



ODH-CPLEX can be used in two ways: it is implemented as a heuristic engine, which can be used on its own; and also within the IBM CPLEX optimizer, within which it can supply and receive solutions from the main CPLEX caller thereby accelerating optimization compared with IBM CPLEX run on its own. The option **Search Mode**  determines which approach is used by ODH-CPLEX.



The ODH-CPLEX engine has a heuristic method for finding an initial feasible solution that it designed to complement, those of CPLEX. Since its main algorithmic procedure works by improving an incumbent feasible solution, getting an initial one is important and may consume a significant part of its total runtime. When used on its own, users should experiment to discover whether ODH-CPLEX or CPLEX’s initial feasible solution methods work best, but within ODH-CPLEX both methods are run in parallel and the winner is chosen automatically.



ODH-CPLEX' principal algorithm works by solving a sequence of sub-models. An innovative aspect of this process is its ability to use the model’s symbolic structure to achieve the sub-model decomposition. It does this by analyzing the symbolic names that the user gives to the decision variables and careful specification of how this should be done this is worthwhile. ODH-CPLEX can work without this analysis, but it usually takes about twice as much runtime. The section :ref:`ODH-CPLEX_-_Specifying_Model_Structure` describes how ODH-CPLEX breaks down the matrix (from the original model) into sub-models.



**Parallel Execution** 

ODH-CPLEX can use multiple simultaneous threads to improved the performance. More information can be found in the section :ref:`ODH-CPLEX_-_Parallel_Execution`.



**Options/Parameters** 

ODH-CPLEX is equipped with parameters that influence the performance of ODH-CPLEX. AIMMS is equipped with options that set the parameters in ODH-CPLEX. ODH-CPLEX has 4 sets of options, namely options that influence:




*   the ODH engine
*   the main CPLEX solve in ODH-CPLEX (if the **Search Mode**  is set to 'Global Solution') or for getting an initial feasible solution (if the **Search Mode**  is set to 'Local Solution')
*   the heuristic sub-model CPLEX solves
*   the heuristic sub-model CPLEX solves in Phase I



The first two categories of options in AIMMS can be set in the options dialog box. The last two categories of options can only be set using a parameter file. (The first two categories of options can also be set using this parameter file.) More information can be found in the section :ref:`ODH-CPLEX_-_Parameter_File`.



The sections :ref:`ODH_to_AIMMS_Mapping` and :ref:`AIMMS_to_ODH_Mapping` contain mappings between the ODH-CPLEX parameters and the AIMMS options for ODH-CPLEX.



**Features** 

ODH-CPLEX 5.3 uses CPLEX version 20.1 underneath. ODH-CPLEX supports many of the CPLEX 20.1 features, including:




*   Callback procedures (except the lazy constraint callback)
*   Indicator constraints
*   Parallel Concurrent Optimizer
*   Multiple MIP starts
*   Second-order cone constraints (SOCP)
*   Solution pool
*   Special Ordered Sets (SOS)
*   User cuts and lazy constraints



ODH-CPLEX does support lazy constraints that are added to a pool of lazy constraints upfront but not the lazy constraint callback. We refer to the CPLEX 20.1 Help for more information regarding the above features.



**Learn more about** 

*	`ODH-CPLEX <https://www.optimizationdirect.com/>`_ (Internet link)
*	:ref:`ODH_to_AIMMS_Mapping`  
*	:ref:`AIMMS_to_ODH_Mapping`  
*	:ref:`Options_AIMMS_Execution_Options`  
*	:ref:`ODH-CPLEX_-_Parallel_Execution` 
*	:ref:`ODH-CPLEX_-_Parameter_File` 
*	:ref:`option-ODHCPLEX-search_mode`  
*	:ref:`ODH-CPLEX_-_Specifying_Model_Structure` 
