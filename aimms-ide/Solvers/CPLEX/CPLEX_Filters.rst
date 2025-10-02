.. _CPLEX_Filters:

Solution Pool Filters
=====================

Filtering allows you to control properties of the solutions generated and stored in the solution pool. CPLEX provides two predefined ways
to filter solutions:

*	If you want to filter solutions based on their difference as compared to a reference solution, use a *diversity filter*.
*	If you want to filter solutions based on their validity in an additional linear constraint, use a *range filter*.

Filters are only used if the option **Do Populate** is switched on.


**Diversity filter** 

A diversity filter allows you to generate solutions that are similar to (or different from) a set of reference values that you specify for
a set of binary variables. In particular, you can use a diversity filter to generate more solutions that are similar to an existing solution
or to an existing partial solution. Several diversity filters can be used simultaneously, for example, to generate solutions that share the
characteristics of several different solutions. 

In AIMMS, a constraint is used as a diversity filter if the constraint has property 'IsDiversificationFilter'. In a diversity filter the Abs
function is used to measure the distance from a given binary variable, and all variables should only occur as the argument of an Abs function.


**Range filter** 

A range filter allows you to generate solutions that obey a new constraint, specified as a linear expression within a range. 

Range filters can be used to express diversity constraints that are more complex than the standard form implemented by diversity filters.
In particular, range filters also apply to general integer variables, semi-integer variables, continuous variables, and semi-continuous
variables, not just to binary variables.


In AIMMS, a constraint is used as a range filter if the constraint has property 'IsRangeFilter'. In a range filter all variables should be
specified as a linear expression.


**Learn more about** 

*	:ref:`CPLEX_Solution_Pool`  
*	:ref:`option-CPLEX-do_populate`  
