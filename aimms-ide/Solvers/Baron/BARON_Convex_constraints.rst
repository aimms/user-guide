

.. _Baron_Convex_constraints:


Convex Constraints
==================

BARON provides the modeler with the flexibility of explicitly identifying convex constraints. Providing BARON with this information can speed up the solution process, often by several orders of magnitude.



In case BARON is unable to determine the convexity of a constraint automatically, the user has to do the identification. This can be done by either setting the .Convex suffix of a constraint, or by using the AIMMS routine GMP::Row::SetConvex.



**Note** 

*	Falsely identifying a constraint as being convex can result in BARON not finding the true global optimum.




**Learn more about** 

*	:ref:`sec:var.constr`  
*	:any:`GMP::Row::SetConvex`




**References** 

*	Tawarmalani, M. and N. V. Sahinidis, A polyhedral branch-and-cut approach to global optimization, Mathematical Programming, Series B **103**  (2005), pp. 225-249.
