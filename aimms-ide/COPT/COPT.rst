
COPT
========

**Description** 

COPT is a tool for solving linear optimization problems. Such problems are conventionally written like this:



``Minimize (or Maximize)`` c1x1 + c2x2 + ... + cnxn

``Subject to:`` 

a11x1 + a12x2 + … + a1nxn ~ b1

a21x1 + a22x2 + … + a2nxn ~ b2

  …

am1x1 + am2x2 + … + amnxn ~ bm

l1 <= x1 <= u1, …, ln <= xn <= un



where,

x is the vector of variables,

a, b, and c are real numbers,

l and u are vectors of lower and upper bounds, and

~ can be either <=, >=, or =.



Some of the lower bounds may be –inf and some of the upper bounds may be inf. The scalar value n will denote the number of variables and m the number of equations. COPT can handle ranged constraints, i.e., constraints with both a finite lower and upper bound.



In the most basic linear optimization problem, the variables of the objective function are continuous in the mathematical sense, with no gaps between real values. COPT can also be used for solving linear programming problems in which some or all of the variables must assume integer values in the solution. Such problems are known as mixed integer programs or MIPs.



COPT can also handle certain problems in which the objective function is not linear but quadratic. Such a problem is known as quadratic program or QP if the constraints are linear, and it is known as quadratically constrained program or QCP if some of the constraints are quadratic. COPT can also be used for some types of second-order cone constraints, and it can be used to solve programs with a non-convex quadratic objective and/or non-convex quadratic constraints; see the section about :ref:`COPT_Quadratic_Programs` .



COPT is equipped with parameters that influence the performance of COPT. AIMMS is equipped with options that set the parameters in COPT. Options in AIMMS can be set in the options dialog box.



In COPT it is possible to use a solution as a MIP start by setting the option **MIP Start** . COPT also supports :ref:`COPT_Multiple_MIP_Starts` .



COPT can generate multiple solutions to a MIP problem. This is described in the section :ref:`COPT_Solution_Pool` .



**Parallel COPT** 

COPT has a parallel optimizer for solving MIP problems. This parallel optimizer is implemented to run on hardware platforms with parallel processors. To invoke the parallel optimizer you have to set the option **Thread Limit** .



**Postsolve** 

When solving a problem COPT allows variables to slightly violate their bounds as specified by some (feasibility) tolerance. When solving a MIP problem, COPT does not round the found integer variable values to the nearest integer value. Instead the solver returns values which are considered to be integer within some (integrality) tolerance. For these reasons AIMMS offers a postsolve step during which integer variables are fixed to the nearest integer and/or variables outside their bounds are fixed to the nearest bound. In case of a MIP, this results in a problem in which all integer variables are fixed, and therefore it can be solved as a LP problem. See the new general solvers option **Postsolve**  for more information.



**Learn more about** 

*	`COPT <https://www.cardopt.com/copt>`_ (Internet link)
*	:ref:`COPT_to_AIMMS_Mapping`  
*	:ref:`COPT_AIMMS_to_COPT_Mapping`  
*	:ref:`Options_AIMMS_Execution_Options`  
*	:ref:`COPT_Multiple_MIP_Starts` 
*	:ref:`COPT_Quadratic_Programs` 
*	:ref:`COPT_Solution_Pool` 
*	:ref:`COPT_SOS_Types` 
*	:ref:`COPT_Troubleshooting` 
*	:ref:`COPT_MIP_-_MIP_start` 
*	:ref:`Options_Postsolve_-_Postsolve` 
*	:ref:`COPT_Parallel_-_Thread_limit` 
