

.. _CPX221_SOCP:
.. _CPLEX_SOCP:


SOCP
====

CPLEX 22.1 solves a large class of models with quadratic terms among the constraints. CPLEX transforms quadratic constraints automatically into a quadratic constraint of this type:



*	x'Qx <= e where e is a linear expression and Q is positive semi-definite (PSD),




or a second-order cone constraint of one of these types:




*	x'Qx <= y² where y >= 0 and Q is PSD,



*	x'Qx <= yz where y >= 0 , z >= 0, and Q is PSD.




A model containing a constraint of one of the last two types is a second-order cone programming (SOCP) model. The model can contain continuous and/or integer variables.





CPLEX 22.1 can obtain the dual values (i.e., shadow prices) and reduced costs of QCP and SOCP models. However, CPLEX 22.1 does not provide the dual values for quadratic and second-order cone constraints.

