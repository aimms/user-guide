

.. _COPT60_Solution_Pool:
.. _COPT_Solution_Pool:


Solution Pool
=============

The solution pool stores multiple solutions to a mixed integer programming (MIP) model. With this feature, you can direct the algorithm to generate multiple solutions in addition to the optimal solution. The option **Pool Size**  determines the amount of solutions that are stored in the solution pool. By default, none is stored.



By default, the COPT MIP solver will try to find one proven optimal solution to your model. It will typically find multiple sub-optimal solutions along the way. However, these solutions aren't produced in a systematic way. The set of solutions that are found depends on the exact path the solver takes through the MIP search. You could solve a MIP model once, obtaining a set of interesting sub-optimal solutions, and then solve the same problem again with different option settings, and find only the optimal solution.



**Accessing a solution in the solution pool** 

All solutions in the solution pool will be stored in the solution repository of the mathematical program. At position 1 of that solution repository the best solution is stored, at position 2 the solution with the second best objective value, and so on. Solutions in the solution repository can be send to the model identifiers by using the AIMMS routine GMP::Solution::SendToModel. For example, with



	GMP::Solution::SendToModel( 'frac1', 2 );



the second best solution for the mathematical program 'frac1' will be send to the model identifiers.



**Learn more about** 

*	:ref:`COPT_MIP_-_Pool_size` 
*	:any:`GMP::Solution::SendToModel`
