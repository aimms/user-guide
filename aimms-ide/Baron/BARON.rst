BARON
========

**Description** 

BARON (Branch And Reduce Optimization Navigator) is a solver specifically designed for solving Global optimization problems, 
in particular nonlinear programming (NLP) problems and mixed integer nonlinear programming (MINLP) problems. 

MINLP problems can be expressed in the following form:

.. math::

    \begin{array}{ll}
    \text{Minimize:} & f(x,y) \\
    \text{Subject to:} & \\
    & h(x,y) \le b \\
    & Cx + Dy \le d \\
    & l_1 \le x \le u_1, \quad x \text{ continuous} \\
    & l_2 \le y \le u_2, \quad y \text{ integer}
    \end{array}


.. Minimize: f(x,y)
.. 
.. Subject to:
.. 
.. h(x,y) <= b
.. 
.. Cx + Dy <= d
.. 
.. l1 <= x <= u1, x continuous
.. 
.. l2 <= y <= u2, y integer



where,

*   :math:`x` is the vector of continuous variables,
*   :math:`y` is the vector of integer variables,
*   :math:`l1` and :math:`u1` are vectors of lower and upper bounds on the continuous variables,
*   :math:`l2` and :math:`u2` are vectors of lower and upper bounds on the integer variables,
*   :math:`f` is a differentiable (nonlinear) function: the objective function,
*   :math:`h` is a vector of differentiable nonlinear functions,
*   :math:`b` is a vector of right-hand side values of the nonlinear constraints,
*   :math:`C` and :math:`D` are matrices for the continuous and integer variables, and
*   :math:`d` is a vector of right-hand side values of the linear constraints.



The problem is called a nonlinear programming (NLP) problem if there are no integer variables.



The development of the BARON global optimization system began in the early 1990s in an effort to integrate constraint programming and optimization techniques within the branch-and-bound framework for the global optimization of nonconvex nonlinear and mixed-integer nonlinear programs. The approach relies on constraint propagation, interval analysis, and duality to draw inferences regarding ranges of integer and continuous variables in an effort to expedite the traditional branch-and-bound algorithm for global optimization problems. Because considerable emphasis is placed on the reduction of variable bounds, the overall methodology is referred to as branch-and-reduce.



While traditional NLP and MINLP algorithms are guaranteed to converge only under certain convexity assumptions, BARON guarantees to provide global optima under fairly general assumptions. These include the availability of finite lower and upper bounds on the variables and their expressions in the NLP or MINLP to be solved.



BARON requires that all nonlinear variables and expressions in the mathematical program are bounded from below and above. It is important that the user provides finite lower and upper bounds on all variables. Providing finite bounds on the variables does not guarantee finite bounds on the nonlinear expressions in the model. For instance, consider the term 1/x for x in [0,1], which has finite lower and upper bounds, but is unbounded. It is important to provide bounds for the variables such that all expressions have finite values.



If the user does not include variable bounds that guarantee that all expressions have finite values, BARON's preprocessor will attempt to infer appropriate bounds from problem constraints. If this step fails, global optimality of the solutions provided is not guaranteed. Occasionally, because of the lack of bounds no numerically stable lower bounding problems can be constructed, in which case BARON may terminate.



BARON cannot handle constraints that contain goniometric functions or ErrorF functions. Furthermore, BARON cannot handle constraints that contain an if-then-else statement with a variable in the condition. BARON also cannot handle constraints with a reference to an external function. Also the following special functions cannot be handled by BARON: Min, Max, Mod, Div, Sign, Degrees, Radians, Ceil, Floor, Trunc, Round and MapVal, and the distribution functions. Also the operator /$ cannot be handled.



BARON cannot handle powers of the form xy where x and y are variables but AIMMS will automatically reformulate such an expression to the equivalent expression exp(y * log(x)). You should ensure that the level value of x is strictly larger than 0, before the solve statement, otherwise you might get a derivative evaluation error.



BARON is equipped with parameters that influence the performance of BARON. AIMMS is equipped with options that set the parameters in BARON. Options in AIMMS can be set in the options dialog box.



One of the most important options is the option **Maximal Variable Bound** . If one of the variables has no upper bound then the value of this option will be passed to BARON as the upper bound of that variable. If that variable has no lower bound then minus that value will be passed. BARON might sometimes return 'infeasible' if the value of this option is set too low.



BARON can use branching priorities for continuous and integer variables; see the section about :ref:`Baron_Variable_Priorities` .



If BARON declares a problem as infeasible, it has the capability to identify a subset of the constraints that are infeasible and become feasible once any one of them is eliminated. This, so-called, irreducibly inconsistent system (IIS) can be produced by BARON for all types of problems handled by BARON, including linear and nonlinear, continuous and integer, convex and nonconvex. The option **Compute IIS**  can be used to identify an IIS.



**Presolving** 

AIMMS contains a nonlinear presolve algorithm with the goal to reduce the size of the problem and to tighten the variable bounds, which may help BARON to solve nonlinear problems faster. The nonlinear presolve algorithm is switched off by default. To use it you should switch on the AIMMS general solvers option **Nonlinear Presolve** .



**Remark** 

BARON does not use the AIMMS general solvers options **MIP Relative Optimality Tolerance** , **MIP Absolute Optimality Tolerance**  and **Cutoff** ; instead the BARON options **Relative Termination Tolerance** , **Absolute Termination Tolerance**  and **Cut Off**  are used.



**Important Notice** 

When using BARON, the general solvers option **Combine Quadratic Terms**  should be turned off. When this option is turned on, quadratic terms in constraint definitions will be combined by the AIMMS translator before passing the constraint to the solver. For instance, if the definition of some constraint contains the quadratic term x * z + y * z then this will be passed as (z + y) * x if this option is turned on, and as x * z + y * z if this option is turned off. In general, BARON is more efficient if this option is turned off. Therefore we advice to switch this option off when using BARON.



**Learn more about** 

*   `BARON <https://minlp.com>`_ (Internet link)
*   :ref:`BARON_to_AIMMS_Mapping`  
*   :ref:`AIMMS_to_BARON_Mapping`  
*   :ref:`Options_AIMMS_Execution_Options`  
*   :ref:`Baron_Convex_constraints` 
*   :ref:`Baron_Relaxation_only_constr` 
*   :ref:`Baron_General_-_Maximal_variable_bound` 
*   :ref:`Options_NonlinPres_-_NonlinearPresolve` 
*   :ref:`Options_Interface-CombineQuadratic`  
*   :ref:`Baron_Variable_Priorities` 
*   :ref:`Baron_Improving_MINLP_Performance` 
*   :ref:`Baron_Termination_-_Absolute_terminat` 
*   :ref:`Baron_General_-_Compute_IIS` 
*   :ref:`Baron_General_-_Cutoff` 
*   :ref:`Baron_Termination_-_Relative_terminat` 






