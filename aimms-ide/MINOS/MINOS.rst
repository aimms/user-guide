MINOS
=====

**Description** 

MINOS is a FORTRAN-based computer program designed to solve nonlinear programming problems expressed in the following form:




.. list-table::

   * - ``minimize`` (x)
     - Fobj(x) 
   * - ``subject to`` 
     - L <= F(x) <= U
   * - 
     - l <= x <= u




where

x is the vector of variables,

l and u are vectors of lower and upper bounds on the variables,

Fobj is a differentiable (nonlinear) function,

F is a vector of differentiable nonlinear functions, and

L and U are vectors of lower and upper bounds on F.



Some of the lower bounds may be – ¥ and some of the upper bounds may be + ¥. The scalar value n will denote the number of variables and m the number of constraints (i.e., the size of vector F) when they appear in this topic.



MINOS has been invented by Bruce Murtagh and Michael Saunders, and has been distributed by Stanford University.



To solve nonlinear programming problems, MINOS uses a projected augmented Lagrangian algorithm. A brief description of the main features of the algorithm used in MINOS can be found below.



The relationship between the model formulation above and the AIMMS model is simple, the inequalities defined in AIMMS with <= or >= are converted into equalities by the addition of properly bounded slacks. Slacks with lower and upper bounds of zero are added to all AIMMS equalities to ensure that the Jacobian matrix - the matrix of derivatives of the functions in g with respect to x - has full row rank. All these slacks are, together with the normal AIMMS variables, included in x. The vector l represents the lower bounds as defined in AIMMS, either with the range specified at declaration, or explicitly with the '.lower' qualifier, and any bounds on the slacks. Similarly, u represents upper bounds as defined in AIMMS and any bounds on the slacks. The function g represents the non-constant terms of the AIMMS equations themselves; non-constant terms appearing on the right-hand side are moved to the left-hand side.



MINOS is equipped with parameters that influence the performance of MINOS. AIMMS is equipped with options that set the parameters in MINOS. Options in AIMMS can be set in the options dialog box.



Note that the AIMMS general solvers option **Iteration Limit**  defines (in case of MINOS) a limit on the number of major iterations. It is intended to guard against an excessive number of linearizations of the constraints.



**Presolving** 

AIMMS contains a nonlinear presolve algorithm with the goal to reduce the size of the problem and to tighten the variable bounds, which may help MINOS to solve nonlinear problems faster. MINOS is a local solver, i.e., the solution found by the MINOS is a local solution and cannot be guaranteed to be a global solution. The presolve algorithm may help the solver in finding a better solution. A local solver might sometimes fail to find a solution and then it is not always clear whether that is caused by the problem being infeasible or by the solver failing to find a solution for a feasible problem. The presolve algorithm may reveal inconsistent constraints and/or variable bounds and hence identify a problem as infeasible.



The nonlinear presolve algorithm is switched off by default. To use it you should switch on the AIMMS general solvers option **Nonlinear Presolve** .



**Learn more about** 

*	`MINOS <https://web.stanford.edu/group/SOL/home_software.html>`_ (Internet link)
*	:ref:`MINOS_MINOS_to_AIMMS_Mapping`  
*	:ref:`MINOS_AIMMS_to_MINOS_Mapping`  
*	:ref:`MINOS_Description_of_MINOS_Algorithm` 
*	:ref:`Options_AIMMS_Execution_Options`  
*	:ref:`Options_Stop_Criteria_-_Iteration_Limi`  
*	:ref:`Options_NonlinPres_-_NonlinearPresolve` 
