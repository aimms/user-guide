CPLEX
==========

**Description** 

CPLEX is a tool for solving, first of all, linear optimization problems. Such problems are conventionally written like this:



``Minimize (or Maximize)`` :math:`c_{1}x_{1} + c_{2}x_{2} + \ldots + c_{n}x_{n}`

``Subject to:`` 

:math:`
a_{11}x_{1} + a_{12}x_{2} + \ldots + a_{1n}x_{n} \sim b_1 \\
a_{21}x_{1} + a_{22}x_{2} + \ldots + a_{2n}x_{n} \sim b_2 \\
\: \ldots \\
a_{m1}x_{1} + a_{m2}x_{2} + \ldots + a_{mn}x_{n} \sim b_m \\
l_1 <= x_1 <= u_1 \\
\: \ldots \\
l_n <= x_n <= u_n
`

where,
* :math:`x` is the vector of variables,
* :math:`a`, :math:`b`, and :math:`c` are real numbers,
* :math:`l` and :math:`u` are vectors of lower and upper bounds, and
* :math:`\sim` can be either <=, >=, or =.

Some of the lower bounds may be –inf and some of the upper bounds may be inf. The scalar value :math:`n` denotes the number of variables and :math:`m` the number of equations.

In the most basic linear optimization problem, the variables of the objective function are continuous in the mathematical sense, with no gaps between real values. CPLEX can also be used for solving linear programming problems in which some or all of the variables must assume integer values in the solution. Such problems are known as mixed integer programs or MIPs.

CPLEX can handle problems with multiple objectives; see the section :ref:`CPLEX_Multi_Objective_Optimization` .

CPLEX can also handle certain problems in which the objective function is not linear but quadratic. 
Such a problem is known as quadratic program or QP if the constraints are linear, and it is known as quadratically constrained program or QCP if some of the constraints are quadratic. 
(No other type of constraints is allowed.) 
CPLEX can also handle QP and QCP problems in which some or all variables must be integer. Such problems are called mixed integer quadratic programs (MIQP) and mixed integer quadratically constrained programs (MIQCP) respectively. 
CPLEX can also be used for some types of second-order cone constraints; see the section about :ref:`CPLEX_SOCP` .

CPLEX also offers a network optimizer aimed at a special class of linear problems with network structure. 
CPLEX can optimize such problems as ordinary linear programs, but if CPLEX can extract all or part of the problem as a network, 
then CPLEX will apply a more efficient network optimizer to that part of your problem and use the partial solution it finds there to construct an advanced starting point to optimize the rest of the problem.

CPLEX is equipped with parameters that influence the performance of CPLEX. 
AIMMS is equipped with options that set the parameters in CPLEX. 
Options in AIMMS can be set in the options dialog box.

CPLEX can perform a minimum-cost relaxation in order to make an infeasible model feasible. 
More information about relaxing infeasible models can be found in the section :ref:`CPLEX_Feasibility_Relaxation` .

In CPLEX it is possible to use a partial solution as a MIP start by setting the option **Advanced Start** . 
CPLEX also supports :ref:`CPLEX_Multiple_MIP_Starts` .

CPLEX supports several types of callback procedures which allow you to monitor closely and to guide the behavior of the CPLEX optimizers. 
In particular, callbacks allow user code to be executed regularly during an optimization run. 
See the section :ref:`CPLEX_Threads_search_strat_and_callb`  and the option **Use Generic Callbacks** .

CPLEX can generate multiple solutions to a MIP problem. 
This is described in the section :ref:`CPLEX_Solution_Pool` .

CPLEX supports the :ref:`CPLEX_Tuning_Tool` , a utility to aid you in improving the performance of your optimization applications, 
analyzes a model or a group of models and suggests a suite of option settings for you to use that provide better performance than the default option settings for your model or group of models.

CPLEX can use a Benders decomposition algorithm to solve linear problems; 
this is described in the section :ref:`CPLEX_Benders_Decomposition` .

CPLEX can provide information about the quality of a solution that it found by solving a problem; 
this is controlled by the option :ref:`CPLEX_General_-_Display_Solution_Statistics` .

**Parallel CPLEX** 

CPLEX supports several parallel optimizers: Parallel Barrier, Parallel MIP and the Concurrent Optimizer. 
They are implemented to run on hardware platforms with parallel processors. 
The easiest way to let the CPLEX optimizers invoke parallel threads is to set the option **Global Thread Limit** . 
CPLEX can use parallel threads for solving MIP models and, if the barrier algorithm is used, for solving LP, QP and QCP models. 
The Concurrent Optimizer is described in the section :ref:`CPLEX_Parallel_Concurrent_Optimizer` .

**Deprecated postsolve options** 

The postsolve step for linear models has been moved from the solver interface of CPLEX to AIMMS. The postsolve options of CPLEX have been replaced by general solvers options with similar names. See the new general solvers option **Postsolve**  for more information.



**Supported computers** 

CPLEX requires that your computer's CPU supports SSE2. SSE2 was first introduced by Intel in 2001, and AMD added support for SSE2 in 2003.



**Learn more about** 

*	`CPLEX <https://www.ibm.com/products/ilog-cplex-optimization-studio/>`_ (Internet link)
*	:ref:`CPLEX_CPLEX_to_AIMMS_Mapping`  
*	:ref:`CPLEX_AIMMS_to_CPLEX_Mapping`  
*	:ref:`Options_AIMMS_Execution_Options`  
*	:ref:`CPLEX_Benders_Decomposition` 
*	:ref:`CPLEX_Threads_search_strat_and_callb` 
*	:ref:`CPLEX_Indicator_Constraints` 
*	:ref:`CPLEX_Multi_Objective_Optimization` 
*	:ref:`CPLEX_Multiple_MIP_Starts` 
*	:ref:`CPLEX_Parallel_Concurrent_Optimizer` 
*	:ref:`CPLEX_SOCP` 
*	:ref:`CPLEX_Solution_Pool` 
*	:ref:`CPLEX_SOS_Types` 
*	:ref:`CPLEX_SubMIP` 
*	:ref:`CPLEX_Troubleshooting` 
*	:ref:`CPLEX_Tuning_Tool` 
*	:ref:`CPLEX_User_Cuts_and_Lazy_Constraints` 
*	:ref:`CPLEX_General_-_AdvancedStart` 
*	:ref:`CPLEX_Benders_-_Benders_Strategy`  
*	:ref:`CPLEX_General_-_Display_Solution_Statistics`  
*	:ref:`CPLEX_Par_-_GlobalThreadLimit` 
*	:ref:`Options_Postsolve_-_Postsolve` 
*	:ref:`CPLEX_MIP_-_Use_Generic_Callbacks` 
