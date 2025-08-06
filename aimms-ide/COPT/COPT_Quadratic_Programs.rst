

.. _COPT60_Quadratic_Programs:
.. _COPT_Quadratic_Programs:


Quadratic Programs
==================

COPT 6.0 can handle both convex quadratic constraints. The default algorithms in COPT 6.0 only accept a few forms of quadratic constraints that are known to have convex feasible regions. Constraints of the following forms are always accepted:



*	x'Qx <= e where e is a linear expression and Q is positive semi-definite (PSD),



*	x'Qx <= y² where y >= 0 and Q is PSD,



*	x'Qx <= yz where y >= 0 , z >= 0, and Q is PSD.




A model containing a constraint of one of the last two types is a second-order cone programming (SOCP) model. The model can contain continuous and/or integer variables.




