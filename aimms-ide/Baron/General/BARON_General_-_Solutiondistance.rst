

.. _option-Baron-solution_distance:


Solution distance
=================



:Type:	Floating point number	
:Range:	[1e-11,1.0]	
:Default:	1e-4	



This option determines the separation distance between the solutions if the value of the option **Number of Best Solutions**  is greater than 1. For combinatorial problems, solutions are isolated. For continuous problems, solution points within a distance that does not exceed the value of this options are indistinguishable.



The distance between two solutions x and y is calculated according to the infinity norm (or maximum norm):



``|| x - y ||`` ¥ = max ( | x1 - y1 ``|, ..., |`` xn - yn | ).



**Learn more about** 

*	:ref:`option-Baron-number_of_best_solutions` 



