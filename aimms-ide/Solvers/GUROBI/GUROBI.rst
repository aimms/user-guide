.. _SolverGurobi:

Gurobi
===========

**Description** 

Gurobi is a tool for solving linear optimization problems and nonlinear optimization problems. Linear optimization problems are conventionally written like this:

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
The scalar value :math:`n` denotes the number of variables and :math:`m` the number of equations.

The optimization problem can be maximized instead of minimized.

Gurobi can handle ranged constraints, i.e., constraints with both a finite lower and upper bound, 
but it cannot handle (GMP) updates on the left-hand-side or right-hand-side of a ranged constraint.

In the most basic linear optimization problem, the variables of the objective function are continuous in the mathematical sense, with no gaps between real values. 
Gurobi can also be used for solving linear programming problems in which some or all of the variables must assume integer values in the solution. 
Such problems are known as mixed integer programs or MIPs.

Gurobi can handle problems with multiple objectives; see the section :doc:`GUROBI_Multi-Objective_Optimization <GUROBI_Multi-Objective_Optimization>`.

Gurobi can also handle certain problems in which the objective function is not linear but quadratic. 
Such a problem is known as quadratic program or QP if the constraints are linear, 
and it is known as quadratically constrained program or QCP if some of the constraints are quadratic. 
Gurobi can also handle QP and QCP problems in which some or all variables must be integer. 
Such problems are called mixed integer quadratic programs (MIQP) and mixed integer quadratically constrained programs (MIQCP) respectively. 
Gurobi can also be used for some types of second-order cone constraints, and it can be used to solve programs with a non-convex quadratic objective and/or
non-convex quadratic constraints; see the section about :doc:`GUROBI_Quadratic_Programs <GUROBI_Quadratic_Programs>`.

Gurobi can also handle problems in which the objective function and/or some or all of the constraints are nonlinear. It can handle nonlinear problems using
continuous variables only (NLP) and nonlinear problems in which some or all variables must be integer (MINLP). Both problem types are solved to global
optimality using a branch-and-bound algorithm. (Note: for some models both QCP and NLP are fitting model types, e.g., if the model only contains quadratic
constraints and a linear objective. In that case the methods used by Gurobi for solving the model as QCP or NLP will be different.)

Gurobi can perform a minimum-cost relaxation in order to make an infeasible model feasible. 
More information about relaxing infeasible models can be found in the section :doc:`GUROBI_FeasRelax_Feasibility_Relaxation <GUROBI_FeasRelax_Feasibility_Relaxation>`.

In Gurobi it is possible to use a solution as a MIP start by setting the option **MIP Start**. 
Gurobi also supports :doc:`GUROBI_Multiple_MIP_Starts <GUROBI_Multiple_MIP_Starts>`.
Alternatively, you can use :doc:`GUROBI_Hints <GUROBI_Hints>` for variables in a MIP model. 
MIP starts and Hints can also be used for NLP and MINLP.

Gurobi can generate multiple solutions to a MIP problem. This is described in the section :doc:`GUROBI_Solution_Pool <GUROBI_Solution_Pool>`.


**Options** 

Gurobi is equipped with parameters that influence the performance of Gurobi. AIMMS is equipped with options that set the parameters in Gurobi.
Options in AIMMS can be set in the options dialog box.

A few options that control the termination of the solving process can be modified from within a callback within Gurobi; see the section :doc:`GUROBI_Callback_Settable_Options <GUROBI_Callback_Settable_Options>`.

Gurobi supports the :doc:`GUROBI_Tuning_Tool <GUROBI_Tuning_Tool>`, a utility to aid you in improving the performance of your optimization applications, analyzes a model or
a group of models and suggests a suite of option settings for you to use that provide better performance than the default option settings for your model or group of models.


**Parallel Gurobi** 

Gurobi supports several parallel algorithms, namely parallel MIP, concurrent MIP, concurrent LP and parallel barrier. These parallel algorithms are implemented to run on hardware platforms with parallel processors. The number of threads used by the parallel algorithms is controlled by the option **Thread Limit**.



**Postsolve** 

When solving a problem Gurobi allows variables to slightly violate their bounds as specified by some (feasibility) tolerance. When solving a MIP problem, Gurobi does not round the found integer variable values to the nearest integer value. Instead the solver returns values which are considered to be integer within some (integrality) tolerance. For these reasons AIMMS offers a postsolve step during which integer variables are fixed to the nearest integer and/or variables outside their bounds are fixed to the nearest bound. In case of a MIP, this results in a problem in which all integer variables are fixed, and therefore it can be solved as a LP problem. See the new general solvers option **Postsolve**  for more information.



**Running Gurobi on Gurobi Compute Server or Gurobi Cloud** 

Normally AIMMS initializes a Gurobi environment at startup and frees it when AIMMS is closed. The procedures GMP::Solver::InitializeEnvironment and GMP::Solver::FreeEnvironment can be used to initialize and free a Gurobi environment multiple times inside one AIMMS sesstion. This makes it possible to connect and disconnect a Gurobi session running on the Gurobi Compute Server or the Gurobi Cloud.



**Supported computers** 

Gurobi requires that your computer's CPU supports SSE2. SSE2 was first introduced by Intel in 2001, and AMD added support for SSE2 in 2003.



**Learn more about** 

*	`GUROBI <https://www.gurobi.com/>`_ (Internet link)
*	:doc:`GUROBI_to_AIMMS_Mapping <GUROBI_to_AIMMS_Mapping>`  
*	:doc:`AIMMS_to_GUROBI_Mapping <AIMMS_to_GUROBI_Mapping>`  
*	:doc:`AIMMS_Execution_Options <../../Aimms/Options/AIMMS_Execution_Options>`  
*	:doc:`GUROBI_Callback_Settable_Options <GUROBI_Callback_Settable_Options>` 
*	:doc:`GUROBI_FeasRelax_Feasibility_Relaxation <GUROBI_FeasRelax_Feasibility_Relaxation>` 
*	:doc:`GUROBI_Hints <GUROBI_Hints>` 
*	:doc:`GUROBI_Indicator_Constraints <GUROBI_Indicator_Constraints>` 
*	:doc:`GUROBI_Multi-Objective_Optimization <GUROBI_Multi-Objective_Optimization>` 
*	:doc:`GUROBI_Multiple_MIP_Starts <GUROBI_Multiple_MIP_Starts>` 
*	:doc:`GUROBI_Quadratic_Programs <GUROBI_Quadratic_Programs>` 
*	:doc:`GUROBI_Solution_Pool <GUROBI_Solution_Pool>` 
*	:doc:`GUROBI_SOS_Types <GUROBI_SOS_Types>` 
*	:doc:`GUROBI_Troubleshooting <GUROBI_Troubleshooting>` 
*	:doc:`GUROBI_Tuning_Tool <GUROBI_Tuning_Tool>` 
*	:doc:`GUROBI_User_Cuts_and_Lazy_Constraints <GUROBI_User_Cuts_and_Lazy_Constraints>` 
*	:doc:`GUROBI_MIP_-_MIP_Start <MIP/GUROBI_MIP_-_MIP_Start>` 
*	:doc:`Postsolve_-_Postsolve <../../Aimms/Options/Solvers General/Postsolve/Postsolve_-_Postsolve>` 
*	:doc:`GUROBI_Parallel_-_Thread_Limit <Parallel/GUROBI_Parallel_-_Thread_Limit>` 
*	:any:`GMP::Solver::FreeEnvironment`
*	:any:`GMP::Solver::InitializeEnvironment`
