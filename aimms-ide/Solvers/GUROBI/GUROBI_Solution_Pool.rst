.. _GUROBI_Solution_Pool:


Solution Pool
=============

The solution pool stores multiple solutions to a mixed integer programming (MIP) model. With this feature, you can direct the algorithm to generate multiple solutions in addition to the optimal solution.



By default, the Gurobi MIP solver will try to find one proven optimal solution to your model. It will typically find multiple sub-optimal solutions along the way (which can be retrieved using a callback procedure). However, these solutions aren't produced in a systematic way. The set of solutions that are found depends on the exact path the solver takes through the MIP search. You could solve a MIP model once, obtaining a set of interesting sub-optimal solutions, and then solve the same problem again with different option settings, and find only the optimal solution.



If you'd like more control over how solutions are found and retained, the Gurobi Optimizer has a number of options available for this.



There are a few subtleties associated with finding multiple solutions that you should be aware of. For example, the notion of finding the n best solutions can be a bit ambiguous when you have a non-zero optimality tolerance. Also, it isn't obvious whether two solutions should be considered different when the model has continuous variables. We'll discuss these issues later in this section.



**Invoking the solution pool** 

The option **Pool Search Mode**  should be set to a non-default value before a normal solve statement (or before GMP::Instance::Solve) to let Gurobi fill the solution pool. You can use the **Pool Search Mode**  option to control the approach used to find solutions. At its default setting, the MIP search simply aims to find one optimal solution. Setting the option to 'Find additional solutions' causes the MIP search to expend additional effort to find more solutions, but in a non-systematic way. You will get more solutions, but not necessarily the best solutions. Setting the option to 'Find best solutions' causes the MIP to do a systematic search for the n best solutions. For both non-default settings, the **Pool Size**  option sets the target for the number of solutions to find.



The option **Pool Size**  controls the size of the solution pool. Changing this option won't affect the number of solutions that are found; it simply determines how many of those are retained.



If you are only interested in solutions that are within a certain gap of the best solution found, you can set the **Pool Gap**  or **Pool Absolute Gap** option. Solutions that are not within the specified gap are discarded.



**Accessing a solution in the solution pool** 

All solutions in the solution pool will be stored in the solution repository of the mathematical program. At position 1 of that solution repository the best solution is stored, at position 2 the solution with the second best objective value, and so on. Solutions in the solution repository can be send to the model identifiers by using the AIMMS routine GMP::Solution::SendToModel. For example, with



	GMP::Solution::SendToModel( 'frac1', 2 );



the second best solution for the mathematical program 'frac1' will be send to the model identifiers.



**Subtleties and Limitations** 

There are a few subtleties associated with finding multiple solutions that we'll cover now.



**Continuous Variables** 

One subtlety arises when considering multiple solutions for models with continuous variables. Specifically, you may have two solutions that take identical values on the integer variables but where some continuous variables differ. By choosing different points on the line between these two solutions, you actually have an infinite number of choices for feasible solutions to the problem. To avoid this issue, we define two solutions as being equivalent if they take the same values on all integer variables (and on all continuous variables that participate in SOS constraints). A solution will be discarded if it is equivalent to another solution that is already in the pool.



**Optimality Gap** 

The interplay between the optimality gap and multiple solutions can be a bit subtle. When using the default **Pool Search Mode** , a non-zero optimality gap indicates that you are willing to allow the MIP solver to declare a solution optimal, even though the model may have other, better solutions. The claim the solver makes upon termination is that no other solution would improve the incumbent objective by more than the optimality gap. Terminating at this point is ultimately a pragmatic choice - we'd probably rather have the true best solution, but the cost of reducing the optimality gap to zero can often be prohibitive.



This pragmatic choice can produce a bit of confusion when finding multiple optimal solutions. Specifically, if you ask for the n best solutions, the optimality gap plays a similar role as it does in the default case, but the implications may be a bit harder to understand. Specifically, a non-zero optimality gap means that you are willing to allow the solver to declare that it has found the n best solutions, even though there may be solutions that are better than those that were returned. The claim in this case is that any solution not among the reported n best would improve on the objective for the worst among the n best by less than the optimality gap.



If you want to avoid this source of potential confusion, you should set the optimality gap to 0 when using setting 'Find best solutions' for the **Pool Search Mode** .



**Logging** 

If you browse the log from a MIP solve with option **Pool Search Mode**  set to a non-default value, you may see the lower bound on the objective exceed the upper bound. This can't happen with the default **Pool Search Mode**  - if you are only looking for one optimal solution, the search is done as soon as the lower bound reaches the upper bound. However, if you are looking for the n best solutions, you have to prove that the model has no solution better than the nth best. The objective for that nth solution could be much worse than that of the incumbent. In this situation, the log file will include a line of the form:



Optimal solution found at node 123 - now completing solution pool...



**Learn more about** 

*	:ref:`option-GUROBI-pool_absolute_gap` 
*	:ref:`option-GUROBI-pool_gap` 
*	:ref:`option-GUROBI-pool_search_mode` 
*	:ref:`option-GUROBI-pool_size` 
*	:any:`GMP::Solution::SendToModel`
