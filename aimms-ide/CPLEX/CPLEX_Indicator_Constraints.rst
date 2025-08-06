

.. _CPX221_Indicator_Constraints:
.. _CPLEX_Indicator_Constraints:


Indicator Constraints
=====================

An indicator constraint is a new way of expressing relationships among variables by specifying a binary variable to control whether or not a linear constraint takes effect. For example, indicator constraints are useful in problems where there are fixed charges to express only if a given variable comes into play.



So-called Big M formulations often exhibit trickle flow, and at times, they behave unstably. The main purpose of indicator constraints is to avoid the unwanted side-effects of Big M formulations. Generally, the use of indicator constraints is **not** warranted when the unwanted side-effects of Big M formulations are not present.



For example, instead of the following Big M formulation, which relies on the x values summing to less than one billion (a formulation that can cause numeric instability or undesirable solutions in some situations):



	constr01: x1 + x2 + x3 - 1e+9 y <= 0



you can enter the following formulation, where y is a binary variable, using an indicator constraint, like this:



	constr01: y = 0 ®  x1 + x2 + x3 = 0



A model with an indicator constraint introduces no new assumptions about upper bounds.



**Note** 

*	The constraint must be linear; a quadratic constraint is not allowed to be an indicator constraint.
*	Only Big M constraints that are not eliminated by preprocessing should possibly be reformulated as an indicator constraint. The option **Print Presolve Status**  can be used to find out which (Big M) constraints are eliminated by preprocessing.




**Learn more about** 

*	:ref:`CPLEX_Prepr_-_Print_Prslv_Sta` 



