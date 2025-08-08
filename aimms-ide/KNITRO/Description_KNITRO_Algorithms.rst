

.. _Description_KNITRO_Algorithms:
.. _KNITRO_Description_KNITRO_Algorithms:


Description of Knitro Algorithms
================================

Knitro has two Interior Point algorithms, an Active-Set algorithm and a Sequential Quadratic Programming (SQP) algorithm for solving nonlinear optimization problems. By default, Knitro will automatically try to choose the best optimizer for the given problem based on the problem characteristics.



**Interior-Direct** 

If the Hessian of the Lagrangian is ill-conditioned or the problem does not have a large-dense Hessian, it may be advisable to compute a step by directly factoring the KKT (primal-dual) matrix rather than using an iterative approach to solve this system. Knitro offers the Interior-Direct optimizer which allows the algorithm to take Newton-like steps using a direct factorization approach. This algorithm will try to take a direct step at each iteration and will only fall back on the iterative step if the direct step is suspected to be of poor quality, or if negative curvature is detected.



Using the Interior-Direct optimizer may result in substantial improvements over Interior-CG when the problem is ill-conditioned (as evidenced by Interior-CG taking a large number of Conjugate Gradient iterations). We encourage the user to try both options as it is difficult to predict in advance which one will be more effective on a given problem. The Interior-Direct optimizer may be used with the **Feasible Mode**  option.



**Interior-CG** 

Since Knitro was designed with the idea of solving large problems, the Interior-CG optimizer in Knitro offers an iterative Conjugate Gradient approach to compute the step at each iteration. This approach has proven to be efficient in most cases and allows Knitro to handle problems with large, dense Hessians, since it does not require factorization of the Hessian matrix. The Interior-CG optimizer may be used with the **Feasible Mode**  option.



**Active-Set** 

Knitro also features an active-set Sequential Linear-Quadratic Programing (SLQP) optimizer. This optimizer is particularly advantageous when "warm starting" (i.e., when the user can provide a good initial solution estimate, for example, when solving a sequence of closely related problems). This algorithm is also best at rapid detection of infeasible problems. The Active algorithm is efficient and robust for small and medium-scale problems, but is typically less efficient than both the Interior-Direct and Interior-CG algorithms on large-scale problems (problems with many thousands of variables and constraints). Note: The **Feasible Mode**  option is not available for use with the Active optimizer.



**Sequential Quadratic Programming (SQP)** 

The Sequential Quadratic Programming (SQP) algorithm in Knitro is an active-set method that solves a sequence of quadratic programming (QP) subproblems to solve the problem. This method is primarily designed for small to medium scale problems with expensive function evaluations – for example, problems where the function evaluations involve performing expensive black-box simulations and/or derivatives are computed via finite-differencing. The SQP iteration is expensive since it involves solving a QP subproblem. However, it often converges in the fewest number of function/gradient evaluations, which is why this method is often preferable for situations where the evaluations are the dominant cost of solving the model.



We strongly encourage you to experiment with all algorithm options as it is difficult to predict which one will work best on any particular problem.



Knitro offers a crossover feature in which the interior point method switches to the active-set method near the solution, to try to get a more exact solution and provide more exact sensitivity and active-set information. The crossover procedure is controlled by the option **Crossover Iterations Limit** .



**Learn more about** 

*	:ref:`KNITRO_General_-_Algorithm`  
*	:ref:`KNITRO_IP_-_CrossoverIterLimit`  
*	:ref:`KNITRO_IP_-_Feasible_mode`  



