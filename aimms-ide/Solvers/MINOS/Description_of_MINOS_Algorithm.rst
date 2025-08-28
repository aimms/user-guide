

.. _Description_of_MINOS_Algorithm:


Description of MINOS Algorithm
==============================

``Nonlinear constraints`` 

MINOS uses a projected augmented Lagrangian algorithm to solve problems with nonlinear constraints. Such a problem can expressed in the following form:

.. math::

    \begin{array}{ll}
    \text{Minimize} & F(x) + c^Tx + d^Ty \\
    (x,y) & \\
    \text{Subject to} & f(x) + A_1y = b_1 \\
    & A_2x + A_2y = b_2 \\
    & l_x \leq x \leq u_x \\
    & l_y \leq y \leq u_y \\
    \end{array}


MINOS treats linear constraints and bounds specially, but the nonlinear constraints may not be satisfied until an optimal point is reached. In fact,
the constraint functions will almost never be evaluated unless the linear constraints are satisfied. The starting point is an exception; it will satisfy
its bounds, but :math:`f(x)` and the Jacobian matrix :math:`J(x)` will be evaluated at :math:`x_0` regardless of the general linear and nonlinear constraints.



**Major iterations** 

The nature of the solution process can be summarized as follows. A sequence of **major iterations** is performed, each one requiring the solution of a
linearly constrained subproblem. The subproblems contain the original linear constraints and bounds, as well as linearized versions of the nonlinear constraints.
This approximation can be written as

.. math::

    f_a(x,x_k) = f(x_k) + J(x_k) (x - x_k),

or more briefly

.. math::

    f_a = f_k + J_k (x - x_k),

where :math:`x_k` is the estimate of the nonlinear variables at the start of the :math:`k`-th major iteration. The subproblem to be solved takes the form:

.. math::

    \begin{array}{ll}
    \text{Minimize} & F(x) + c^Tx + d^Ty - \lambda_k^T (f - f_a) + 0.5 \rho (f - f_a)^T (f - f_a) \\
    (x,y) & \\
    \text{Subject to} & f_a + A_1y = b_1 \\
    & A_2x + A_2y = b_2 \\
    & l_x \leq x \leq u_x \\
    & l_y \leq y \leq u_y \\
    \end{array}


The objective function is called an **augmented Lagrangian**. The vector :math:`\lambda_k` is an estimate of :math:`\lambda`, the Lagrange multipliers
for the nonlinear constraints. The scalar :math:`\rho` is a penalty parameter, and the term involving :math:`\rho` is a modified quadratic penalty function.
MINOS uses the reduced-gradient algorithm to solve the above subproblem.

Unfortunately, there is no guarantee that the algorithm just described will converge from an arbitrary starting point. The concerned user can influence
the likelihood of convergence in several ways:

1.  By specifying the starting point :math:`x_0` as carefully as possible.
2.  By including sensible upper and lower bounds on all variables.
3.  By specifying a **Penalty Parameter** :math:`\rho` that is higher than the default value, if the problem is suspected of being highly nonlinear.
4.  By specifying a **Damping Parameter** that is lower than the default value, again if the problem is highly nonlinear.


The penalty parameter is initially :math:`2000/m` (with :math:`m` being the number of nonlinear constraints) by default, and it is reduced in stages for later subproblems
when it appears that the sequence {:math:`x_k,\lambda_k`} is converging. In many cases it is safe to specify :math:`\rho = 0` from the beginning, particularly if the
problem is only mildly nonlinear. This may improve the overall efficiency.

**Problem formulation** 

In general, it is worthwhile expending considerable prior analysis to make the constraints completely linear if at all possible. Sometimes a simple transformation
will suffice. Even if the objective function becomes more nonlinear by such a transformation, the advantages of having linear constraints greatly outweigh this.
Similarly, it is important not to move nonlinearities from the objective function into the constraints.

Scaling is a very important matter during problem formulation. A general rule is to scale both the data and the variables to be as close to 1.0 as possible.
When conflicts arise, one should sacrifice the objective function in favor of the constraints. MINOS has the option **Scale Method** to scale constraints and variables automatically.

Finally, upper and lower bounds on the variables (and on the constraints) are extremely useful for confining the region over which optimization has to be performed.
If sensible values are known, they should always be used. They are also important for avoiding singularities in the problem functions. For safety when singularities exist,
the initial point :math:`x_0` should lie within the bounds.


**Learn more about** 

*	:ref:`option-MINOS-damping_parameter`  
*	:ref:`option-MINOS-penalty_parameter`  
*	:ref:`option-MINOS-scale_method`  



