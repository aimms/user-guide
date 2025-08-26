.. _SNOPT_Description_of_SNOPT_Algorithm:


Description of SNOPT Algorithm
==============================

**Constraints and slack variables** 

The upper and lower bounds on the :math:`m` components of :math:`G` are said to define the **general constraints** of the problem. SNOPT converts
the general constraints to equalities by introducing a set of **slack variables** :math:`s`, where :math:`s = (s_1,s_2,\ldots,s_m)^T`. For example,
the linear constraint :math:`5 \leq 2x_1 + 3x_2 \leq \infty` is replaced by :math:`2x_1 + 3x_2 - s_1 = 0` together with the bounded slack
:math:`5 \leq s1 \leq \infty`. The problem defined above can therefore be rewritten in the following equivalent form:

.. math::

    \begin{array}{ll}
    \text{Minimize} & F_{obj}(x) \\
    (x,s) \in \mathbb{R}^n \times \mathbb{R}^m & \\
    \text{Subject to} & F(x) - s = 0 \\
    & l \leq x \leq u \\
    & L \leq s \leq U \\
    \end{array}


**Major iterations** 

The basic structure of SNOPT involves **major** and **minor** iterations. The major iterations generate a sequence of iteration points (:math:`x_k`) that satisfy
the linear constraints and converge to a point that satisfies the first-order condition for optimality. At each iteration a QP subproblem is used to
generate a search direction towards the next iteration point (:math:`x_{k+1}`). The constraints of the subproblem are formed from the nonlinear constraint linearization

.. math::

    F(x_k) + F'(x_k) (x - x_k) - s = 0,


where :math:`F'(x_k)` denotes the **Jacobian matrix**, whose rows are the first derivatives of :math:`F'(x)` evaluated at :math:`x_k`. The QP constraints
therefore comprise the :math:`m` linear constraints 

.. math::

    F'(x_k) x - s = - F(x_k) + F'(x_k) x_k,

where :math:`x` is bounded above and below by :math:`u` and :math:`l`, and :math:`s` by :math:`U` and :math:`L` as before. If the :math:`m \times n`
matrix :math:`A` and :math:`m`-vector :math:`b` are defined as

.. math::

    A = F'(x_k) \quad \text{and} \quad  b = - F(x_k) + F'(x_k) x_k,

then the QP subproblem can be written as


.. math::

    \begin{array}{ll}
    \text{Minimize} & q(x) \\
    (x,s) \in \mathbb{R}^n \times \mathbb{R}^m & \\
    \text{Subject to} & Ax - s = b \\
    & l \leq x \leq u \\
    & L \leq s \leq U \\
    \end{array}


where :math:`q(x)` is a quadratic approximation to a modified Lagrangian function. 



**Minor iterations** 

Solving the QP subproblem is itself an iterative process with the minor iterations of an SQP method being the iterations of the QP method.
At each minor iteration, the constraints :math:`Ax - s = b` are (conceptually) partitioned into the form

.. math::

    Bx_B + Sx_S + Nx_N = b,



Where the **basic matrix** :math:`B` is square and nonsingular. The elements of :math:`x_B`, :math:`x_S` and :math:`x_N` are called the **basic**, **superbasic**
and **nonbasic** variables respectively; they are a permutation of the elements of :math:`x` and :math:`s`. At a QP solution, the basic and superbasic variables
will lie somewhere between their bounds, while the nonbasic variables will be equal to one of their upper or lower bounds. At each iteration, :math:`x_S` is
regarded as a set of independent variables that are free to move in any desired direction, namely one that will improve the value of the QP objective
(or the sum of infeasibilities) The basic variables are then adjusted in order to ensure that (x,s) continues to satisfy :math:`Ax - s = b`.
The number of superbasic variables (denoted by :math:`n_s`) therefore indicates the number of degrees of freedom remaining after the constraints have been satisfied.
In broad terms, :math:`n_s` is a measure of how nonlinear the problem is. In particular, ns will always be zero for LP problems.



If it appears that no improvement can be made with the current definition of :math:`B`, :math:`S` and :math:`N`, a nonbasic variable is selected to be
added to :math:`S`, and the process is repeated with the value of :math:`n_s` increased by one. At all stages, if a basic or superbasic variables encounters one of its
bounds, the variable is made nonbasic and the value of :math:`n_s` is decreased by one.



Associated with each of the :math:`m` equality constraints :math:`Ax - s = b` are the **dual variables** :math:`\pi`. Similary, each variables in :math:`(x,s)`
has an associated reduced gradient :math:`d_j`. The reduced gradients for the variables x are the quantities :math:`g - A^T\pi`, where :math:`g` is the gradient of the QP objective,
and the reduced gradients for the slacks are the dual variables :math:`\pi`. The QP subproblem is optimal if :math:`d_j \leq 0` for all the nonbasic variables at their lower
bounds, :math:`d_j \geq 0` for all nonbasic variables at their upper bounds, and :math:`d_j = 0` for all other variables, including superbasics. In practice, an approximate QP
solution if found by relaxing these conditions on :math:`d_j` (see the option **Optimality Tolerance**).



**The merit function** 

After a QP subproblem has been solved, new estimates of the NP solution are computed using a linesearch on the augmented Lagrangian merit function. The linesearch
determines a step :math:`a_k`, with :math:`0 < a_k \leq 1`, such that the new point gives a sufficient decrease in the merit function.



**Treatment of constraint infeasibilities** 

SNOPT makes explicit allowance for infeasible constraints. Infeasible linear constraints are detected first by minimizing the sum of the general linear constraint
violations subject to the simple bounds. If the linear constraints are infeasible, SNOPT terminates without computing the nonlinear functions. If the linear constraints
are feasible, all subsequent iteration points satisfy the linear constraints. (Such a strategy allows linear constraints to be used to define a region in which the
functions can be safely evaluated.) SNOPT proceeds to solve the NLP as given, using search directions obtained from a sequence of quadratic programming subproblems (see before).



If a QP subproblem proves to be infeasible or unbounded (or if the dual variables p for the nonlinear constraints become to large), SNOPT enters an "elastic" mode
in which the nonlinear constraint violations are added to the objective function and penalized by using a constant. (See the option **Elastic Weight**.) If the
penalty constant is sufficiently large, this is equivalent to minimizing the sum of the nonlinear constraint violations subject to the linear constraints and bounds.



**Learn more about** 

*	:ref:`option-SNOPT-elastic_weight`  
*	:ref:`option-SNOPT-optimality_tolerance`  



