

.. _COPT_Quadratic_Programs:


Quadratic Programs
==================

COPT can handle models with a quadratic objective and/or quadratic constraints, containing continuous and/or integer variables, i.e., QP, MIQP, QCP and MIQCP models. Both convex and non-convex models are supported. The default algorithms in COPT only accept a few forms of quadratic constraints that are known to have convex feasible regions. Constraints of the following forms are always accepted:



*	x'Qx <= e where e is a linear expression and Q is positive semi-definite (PSD),



*	x'Qx <= y² where y >= 0 and Q is PSD,



*	x'Qx <= yz where y >= 0 , z >= 0, and Q is PSD.




A model containing a constraint of one of the last two types is a second-order cone programming (SOCP) model. The model can contain continuous and/or integer variables.





Convex QP and QCP models are solved by the barrier method of COPT. Therefore no basis information is available for these models. The dual values (i.e., shadow prices) and reduced costs are available for convex QP models, but not for models with quadratic constraints.





A model with a non-convex quadratic objective or non-convex quadratic constraints, including quadratic equality constraints, is typically much more expensive to solve. For continuous models (QP and QCP), the option **Nonconvex Strategy**  determines how COPT handles such a model: it can report that the model is non-convex and terminate, search for a local optimum, or search for a global optimum using branch-and-bound. If COPT searches for a local optimum then AIMMS reports the model status 'Locally Optimal'. If COPT searches for a global optimum then a best bound is available, and no dual values and reduced costs are returned. Non-convex MIQP and MIQCP models are always solved to global optimality, regardless of the setting of the option **Nonconvex Strategy**.





COPT cannot handle ranged quadratic constraints, and cannot calculate an Irreducible Inconsistent Subsystem (IIS) for models with quadratic constraints.





**Learn more about**

*	:doc:`General/COPT_General_-_Nonconvex_strategy`



