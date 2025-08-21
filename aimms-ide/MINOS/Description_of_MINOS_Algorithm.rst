

.. _Description_of_MINOS_Algorithm:


Description of MINOS Algorithm
==============================

``Nonlinear constraints`` 

MINOS uses a projected augmented Lagrangian algorithm to solve problems with nonlinear constraints. Such a problem can expressed in the following form:




.. list-table::

   * - ``minimize`` (x,y)T
     - F(x) + cTx + dTy
   * - ``subject to`` 
     - f(x) + A1y = b1
   * - 
     - A2x + A2y = b2
   * - 
     - lx ≤ x ≤ ux
   * - 
     - ly ≤ y ≤ uy




MINOS treats linear constraints and bounds specially, but the nonlinear constraints may not be satisfied until an optimal point is reached. In fact, the constraint functions will almost never be evaluated unless the linear constraints are satisfied. The starting point is an exception; it will satisfy its bounds, but f(x) and the Jacobian matrix J(x) will be evaluated at x0 regardless of the general linear and nonlinear constraints.



**Major iterations** 

The nature of the solution process can be summarized as follows. A sequence of **major iterations**  is performed, each one requiring the solution of a linearly constrained subproblem. The subproblems contain the original linear constraints and bounds, as well as linearized versions of the nonlinear constraints. This approximation can be written as



	fa(x,xk) = f(xk) + J(xk) (x - xk),



or more briefly



	fa = fk + Jk (x - xk),



where xk is the estimate of the nonlinear variables at the start of the k-th major iteration. The subproblem to be solved takes the form:




.. list-table::

   * - ``minimize`` (x,y)T
     - F(x) + cTx + dTy - lkT (f - f) + 0.5 r (f - fa)T (f - fa)
   * - ``subject to`` 
     - fa + A1y = b1
   * - 
     - A2x + A2y = b2
   * - 
     - lx ≤ x ≤ ux
   * - 
     - ly ≤ y ≤ uy




The objective function is called an **augmented Lagrangian** . The vector lk is an estimate of l, the Lagrange multipliers for the nonlinear constraints. The scalar r is a penalty parameter, and the term involving r is a modified quadratic penalty function. MINOS uses the reduced-gradient algorithm to solve the above subproblem.



Unfortunately, there is no guarantee that the algorithm just described will converge from an arbitrary starting point. The concerned user can influence the likelihood of convergence in several ways:


#.  By specifying the starting point x0 as carefully as possible.
#.  By including sensible upper and lower bounds on all variables.
#.  By specifying a **Penalty Parameter**  r that is higher than the default value, if the problem is suspected of being highly nonlinear.
#.  By specifying a **Damping Parameter**  that is lower than the default value, again if the problem is highly nonlinear.



The penalty parameter is initially 2000/m (with m being the number of nonlinear constraints) by default, and it is reduced in stages for later subproblems when it appears that the sequence {xk,lk} is converging. In many cases it is safe to specify r = 0 from the beginning, particularly if the problem is only mildly nonlinear. This may improve the overall efficiency.



**Problem formulation** 

In general, it is worthwhile expending considerable prior analysis to make the constraints completely linear if at all possible. Sometimes a simple transformation will suffice. Even if the objective function becomes more nonlinear by such a transformation, the advantages of having linear constraints greatly outweigh this. Similarly, it is important not to move nonlinearities from the objective function into the constraints.



Scaling is a very important matter during problem formulation. A general rule is to scale both the data and the variables to be as close to 1.0 as possible. When conflicts arise, one should sacrifice the objective function in favor of the constraints. MINOS has the option **Scale Method**  to scale constraints and variables automatically.



Finally, upper and lower bounds on the variables (and on the constraints) are extremely useful for confining the region over which optimization has to be performed. If sensible values are known, they should always be used. They are also important for avoiding singularities in the problem functions. For safety when singularities exist, the initial point x0 should lie within the bounds.



**Learn more about** 

*	:ref:`option-MINOS-damping_parameter`  
*	:ref:`option-MINOS-penalty_parameter`  
*	:ref:`option-MINOS-scale_method`  



