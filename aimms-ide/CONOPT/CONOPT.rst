

CONOPT
======

**Description** 

CONOPT is a Generalized Reduced Gradient (GRG) algorithm specifically designed for large nonlinear programming problems expressed in the following form:


.. math::

    \begin{array}{ll}
    \text{Minimize or Maximize:} & f(x) \\
    \text{Subject to:} & \\
    & G(x) = b \\
    & l \le x \le u
    \end{array}

where,

*   :math:`x` is the vector of variables,
*   :math:`l` and :math:`u` are vectors of lower and upper bounds,
*   :math:`b` is a vector of right-hand side values,
*   :math:`f` is a differentiable (nonlinear) function, and
*   :math:`G` is a vector of differentiable nonlinear functions.



Some of the lower bounds may be :math:`-\infty` and some of the upper bounds may be :math:`\infty`. The scalar value :math:`n` denotes the number of variables and :math:`m` the number of equations when they appear in this topic.



The relationship between the model formulation above and the AIMMS model is simple, the inequalities defined in AIMMS with <= or >= are converted into equalities by the addition of properly bounded slacks. Slacks with lower and upper bounds of zero are added to all AIMMS equalities to ensure that the Jacobian matrix - the matrix of derivatives of the functions in :math:`g` with respect to :math:`x` - has full row rank. All these slacks are, together with the normal AIMMS variables, included in :math:`x`.

The vector :math:`l` represents the lower bounds as defined in AIMMS, either with the range specified at declaration, or explicitly with the '.lo' qualifier, and any bounds on the slacks. Similarly, :math:`u` represents upper bounds as defined in AIMMS and any bounds on the slacks. The function :math:`g` represents the non-constant terms of the AIMMS equations themselves; non-constant terms appearing on the right-hand side are moved to the left-hand side.



CONOPT has been designed for large, sparse models. This means that the dimensions of both :math:`x` and :math:`g` can be large. Indeed, models with over 10,000 equations and variables have been solved successfully. The components used to build CONOPT have been selected under the assumption that the model is sparse, i.e., that each function in :math:`g` depends only on a small fraction of the variables. CONOPT can also be used for denser models, but the performance will suffer significantly.



Information about the algorithm used by CONOPT can be found in the section :ref:`CONOPT_Description_of_CONOPT_Algorithm`.



CONOPT is equipped with parameters that influence the performance of CONOPT. AIMMS is equipped with options that set the parameters in CONOPT. Options in AIMMS can be set in the options dialog box.



**Scaling** 

CONOPT assumes implicitly that the model to be solved is well scaled. In this context well scaled means:




*   Basic and superbasic solution values are expected to be between 0.01 and 100. Nonbasic variables will be at a bound, and the bound values should not be larger than 100.
*   Derivatives (or Jacobian elements) are expected to be between 0.01 and 100. 



Variables become well scaled if they are measured in appropriate units. In most cases you should select the unit of measurement for the variables such that their expected value is between 0.01 and 100. Equations become well scaled if the individual terms are measured in appropriate units. After you have selected units for the variables you should select the unit of measurement for the equations such that the expected values of the individual terms are between 0.01 and 100.



Derivatives will usually be well scaled whenever the variables and equations are well scaled. To see if the derivatives are well scaled, run your model with the general solvers option **Constraint Listing**  set, and look for very small (i.e., close to 0) or very large coefficients in the constraint listing. (The constraint listing is printed in the listing file.) CONOPT computes a measure of the scaling of the Jacobian, both in the initial and in the final point, and if it seems to be large it will be printed in the Message Window. The message looks like:

.. code-block:: text

   ** Warning **    The variance of the derivatives in the initial
                    point is large (= 4.1 ). A better initial
                    point, a better scaling, or better bounds on the
                    variables will probably help the optimization.


The variance is computed as


.. math::

   \sqrt{\frac{\sum_{i} \log (| \text{Jac}(i)|)^2}{N}}


where :math:`Jac(i)` represents the nonzero Jacobian elements and :math:`N` the number of nonzero Jacobian elements in the model. A variance of 4.1 means that Jacobian values outside the range Exp(-4.1) = 0.017 to Exp(+4.1) = 60.3 are about as common as values inside the range. This range is for most models acceptable, while a variance of 5, corresponding to about half the derivatives outside the range Exp(-5) = 0.0067 to Exp(+5) = 148.4, can be dangerous.



**Presolving** 

AIMMS contains a nonlinear presolve algorithm with the goal to reduce the size of the problem and to tighten the variable bounds, which may help CONOPT to solve nonlinear problems faster. 
CONOPT is a local solver, i.e., the solution found by the CONOPT is a local solution and cannot be guaranteed to be a global solution. 
The presolve algorithm may help the solver in finding a better solution. 
A local solver might sometimes fail to find a solution and then it is not always clear whether that is caused by the problem being infeasible or by the solver failing to find a solution for a feasible problem. 
The presolve algorithm may reveal inconsistent constraints and/or variable bounds and hence identify a problem as infeasible.



The AIMMS presolve algorithm is switched off by default. 
To use it you should switch on the AIMMS general solvers option **Nonlinear Presolve** .



**Parallel solves** 

CONOPT 4 is thread-safe and therefore multiple nonlinear mathematical program instances can be solved in parallel using CONOPT 4 (assuming your computer has multiple processors or a multi-core processor). 
The procedure :any:`GMP::SolverSession::AsynchronousExecute` should be used to solve multiple mathematical program instances in parallel.



**Note** 

*	This help is for CONOPT versions 4.0 and 4.1.




**Learn more about** 

*	:ref:`CONOPT_to_AIMMS_Mapping`  
*	:ref:`AIMMS_to_CONOPT_Mapping`  
*	:ref:`Options_AIMMS_Execution_Options`  
*	:ref:`CONOPT_Description_of_CONOPT_Algorithm` 
*	:ref:`CONOPT_Troubleshooting` 
*	:ref:`option-AIMMS-constraint_listing` 
*	:ref:`option-AIMMS-nonlinear_presolve` 
