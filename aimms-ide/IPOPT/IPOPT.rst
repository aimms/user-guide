IPOPT
=====

**Description** 

IPOPT (**I** nterior **P** oint **OPT** imizer) is a software package for large-scale nonlinear optimization. It is designed to find (local) solutions of mathematical optimization problems of the from 


.. math::

    \begin{array}{ll}
    \text{Minimize} & f(x) \\
    x \in \mathbb{R}^n & \\
    \text{Subject to} & L_j \le g_j(x) \le U_j \quad j \in J \\
    & l_i \le x_i \le u_i \quad i \in I
    \end{array}

where

* :math:`x` is the vector of variables,
* :math:`f` is the objective function and :math:`g` is a vector of constraint functions,
* the vectors :math:`L` and :math:`U` denote the lower and upper bounds on the constraints, 
* the vectors :math:`l` and :math:`u` are the bounds on the variables x.

The functions :math:`f(x)` and :math:`g(x)` can be nonlinear and nonconvex, but should be twice continuously differentiable. Note that equality constraints can be formulated in the above formulation by setting the corresponding components of :math:`L` and :math:`U` to the same value.

The optimization problem can be maximized instead of minimized.

IPOPT uses an interior point method, together with a filter linear search procedure. The mathematical details of the algorithm are described in the publication:



Wächter and L. T. Biegler, **On the Implementation of a Primal-Dual Interior Point Filter Line Search Algorithm for Large-Scale Nonlinear Programming** , Mathematical Programming 106(1), pp. 25-57, 2006.



IPOPT is equipped with parameters that influence the performance of IPOPT. AIMMS is equipped with options that set the parameters in IPOPT. Options in AIMMS can be set in the options dialog box.



Note that the general solvers option **Iteration Limit**  is not used by IPOPT. Please use the IPOPT option **Maximum Number of Iterations**  instead.



**COIN-OR** 

IPOPT is an open-source solver and available from COIN-OR. The Computational Infrastructure for Operations Research (COIN-OR) project is an initiative to spur the development of open-source software for the operations research community.



The source code of IPOPT is available at COIN-OR. The code has been written by Carl Laird and Andreas Wächter. The source code of the AIMMS-IPOPT link is available from the AIMMSlinks project at COIN-OR. See the Internet links below.



**Presolving** 

AIMMS contains a nonlinear presolve algorithm with the goal to reduce the size of the problem and to tighten the variable bounds, which may help IPOPT to solve nonlinear problems faster. IPOPT is a local solver, i.e., the solution found by the IPOPT is a local solution and cannot be guaranteed to be a global solution. The presolve algorithm may help the solver in finding a better solution. A local solver might sometimes fail to find a solution and then it is not always clear whether that is caused by the problem being infeasible or by the solver failing to find a solution for a feasible problem. The presolve algorithm may reveal inconsistent constraints and/or variable bounds and hence identify a problem as infeasible.



The nonlinear presolve algorithm is switched off by default. To use it you should switch on the AIMMS general solvers option **Nonlinear Presolve** .



**Learn more about** 

*	`IPOPT <https://coin-or.github.io/Ipopt/>`_ (Internet link)
*	`COIN-OR <https://www.coin-or.org/>`_ (Internet link)
*	`AIMMSlinks <https://github.com/coin-or/AIMMSlinks>`_ (Internet link)
*	:ref:`IPOPT_to_AIMMS_Mapping`  
*	:ref:`IPOPT_AIMMS_to_IPOPT_Mapping`  
*	:ref:`Options_AIMMS_Execution_Options`  
*	:ref:`Options_Stop_Criteria_-_Iteration_Limi`  
*	:ref:`Options_NonlinPres_-_NonlinearPresolve` 
*	:ref:`IPOPT_Termination_-_Maximum_number_of_iterations` 
*	:ref:`IPOPT_Troubleshooting` 
