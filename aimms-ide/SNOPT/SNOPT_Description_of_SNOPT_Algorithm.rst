.. _SNOPT_Description_of_SNOPT_Algorithm:


Description of SNOPT Algorithm
==============================

**Constraints and slack variables** 

The upper and lower bounds on the m components of G are said to define the **general constraints**  of the problem. SNOPT converts the general constraints to equalities by introducing a set of **slack variables**  s, where s = (s1,s2,…,sm)T. For example, the linear constraints 5 <= 2x1 + 3x2 <= + ¥ is replaced by 2x1 + 3x2 – s1 = 0 together with the bounded slack 5 <= s1 <= + ¥. The problem defined above can therefore be rewritten in the following equivalent form:



``minimize`` (x,s)Fobj(x) 

``subject to`` 	F(x) - s = 0,

	l <= x <= u,

	L <= s <= U.



**Major iterations** 

The basic structure of SNOPT involves **major**  and **minor**  iterations. The major iterations generate a sequence of iteration points (xk) that satisfy the linear constraints and converge to a point that satisfies the first-order condition for optimality. At each iteration a QP subproblem is used to generate a search direction towards the next iteration point (xk+1). The constraints of the subproblem are formed from the nonlinear constraint linearization



F(xk) + F'(xk) (x – xk) – s = 0,



Where F'(xk) denotes the **Jacobian matrix** , whose rows are the first derivatives of F(x) evaluated at xk. The QP constraints therefore comprise the m linear constraints 



F'(xk) x - s = - F(xk) + F'(xk) xk,



where x is bounded above and below by u and l, and s by U and L as before. If the m x n matrix A and m-vector b are defined as



A = F'(xk)  and b = - F(xk) + F'(xk) xk,



then the QP subproblem can be written as



``minimize`` (x,s)q(x) 

``subject to`` 	Ax - s = b,

	l <= x <= u,

	L <= s <= U,



where q(x) is a quadratic approximation to a modified Lagrangian function. 



**Minor iterations** 

Solving the QP subproblem is itself an iterative process with the minor iterations of an SQP method being the iterations of the QP method. At each minor iteration, the constraints Ax – s = b are (conceptually) partitioned into the form



BxB + SxS + NxN = b,



Where the **basic matrix**  B is square and nonsingular. The elements of xB, xS and xN are called the **basic** , **superbasic**  and **nonbasic**  variables respectively; they are a permutation of the elements of x and s. At a QP solution, the basic and superbasic variables will lie somewhere between their bounds, while the nonbasic variables will be equal to one of their upper or lower bounds. At each iteration, xS is regarded as a set of independent variables that are free to move in any desired direction, namely one that will improve the value of the QP objective (or the sum of infeasibilities) The basic variables are then adjusted in order to ensure that (x,s) continues to satisfy Ax – s = b. The number of superbasic variables (denoted by ns) therefore indicates the number of degrees of freedom remaining after the constraints have been satisfied. In broad terms, ns is a measure of how nonlinear the problem is. In particular, ns will always be zero for LP problems.



If it appears that no improvement can be made with the current definition of B, S and N, a nonbasic variable is selected to be added to S, and the process I repeated with the value of ns increased by one. At all stages, if a basic or superbasic variables encounters one of its bounds, the variable is made nonbasic and the value of ns is decreased by one.



Associated with each of the m equality constraints Ax – s = b are the **dual variables**  p. Similary, each variables in (x,s) has an associated reduced gradient dj. The reduced gradients for the variables x are the quantities g - ATp, where g is the gradient of the QP objective, and the reduced gradients for the slacks are the dual variables p. The QP subproblem is optimal if dj >= 0 for all the nonbasic variables at their lower bounds, dj <= 0 for all nonbasic variables at their upper bounds, and dj = 0 for all other variables, including superbasics. In practice, an approximate QP solution if found by relaxing these conditions on dj (see the option **Optimality Tolerance** ).



**The merit function** 

After a QP subproblem has been solved, new estimates of the NP solution are computed using a linesearch on the augmented Lagrangian merit function. The linesearch determines a step ak (0 < ak <= 1) such that the new point gives a sufficient decrease in the merit function.



**Treatment of constraint infeasibilities** 

SNOPT makes explicit allowance for infeasible constraints. Infeasible linear constraints are detected first by minimizing the sum of the general linear constraint violations subject to the simple bounds. If the linear constraints are infeasible, SNOPT terminates without computing the nonlinear functions. If the linear constraints are feasible, all subsequent iteration points satisfy the linear constraints. (Such a strategy allows linear constraints to be used to define a region in which the functions can be safely evaluated.) SNOPT proceeds to solve the NLP as given, using search directions obtained from a sequence of quadratic programming subproblems (see before).



If a QP subproblem proves to be infeasible or unbounded (or if the dual variables p for the nonlinear constraints become to large), SNOPT enters an "elastic" mode in which the nonlinear constraint violations are added to the objective function and penalized by using a constant. (See the option **Elastic Weight** .) If the penalty constant is sufficiently large, this is equivalent to minimizing the sum of the nonlinear constraint violations subject to the linear constraints and bounds.



**Learn more about** 

*	:ref:`SNOPT_Advanced_-_Elastic_Weight`  
*	:ref:`SNOPT_Limits_-_Optimality_Tolerance`  



