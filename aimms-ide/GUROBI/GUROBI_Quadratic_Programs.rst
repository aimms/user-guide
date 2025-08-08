.. _GUROBI_Quadratic_Programs:


Quadratic Programs
==================

Gurobi can handle both convex and non-convex quadratic constraints. The default algorithms in Gurobi only accept a few forms of quadratic constraints that are known to have convex feasible regions. Constraints of the following forms are always accepted:



*	x'Qx <= e where e is a linear expression and Q is positive semi-definite (PSD),



*	x'Qx <= y² where y >= 0 and Q is PSD,



*	x'Qx <= yz where y >= 0 , z >= 0, and Q is PSD.




A model containing a constraint of one of the last two types is a second-order cone programming (SOCP) model. The model can contain continuous and/or integer variables.





If all quadratic constraints are convex then Gurobi can obtain the dual values (i.e., shadow prices) and reduced costs of QCP and SOCP models if the option **QCP Dual Values**  is switched on.





Solving a model with non-convex quadratic constraints is typically much more expensive. To avoid accidentally solving a much harder problem than may have been intended, Gurobi rejects such constrains by default. To solve a model with non-convex quadratic constraints the option **Nonconvex Strategy**  should be used.





**Learn more about** 

*	:ref:`GUROBI_Quadratic_-_Nonconvex_Strategy` 
*	:ref:`GUROBI_Quadratic_-_QCP_Dual_Values` 



