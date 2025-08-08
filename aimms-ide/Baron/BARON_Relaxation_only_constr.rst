

.. _Baron_Relaxation_only_constr:


Relaxation-only Constraints
===========================

A problem formulation can often be strengthened by adding nonlinear constraints. These additional constraints can be used by BARON to strengthen the lower bounding step of the algorithm. Examples of such constraints are



*	Constraints from the reformulation-linearization technique RLT, and
*	First-order optimality conditions for unconstrained global optimization problems.




A potential complication is that these nonlinear constraints may make local search difficult. For that reason it is possible for the user to indicate this kind of constraints as being relaxation-only constraints. That is, a constraint that is identified as a relaxation-only constraint will be used by BARON to strengthen the lower bounding step of the algorithm, but will be ignored when performing a local search. In AIMMS, a constraint can be identified as relaxation-only by either setting the .RelaxationOnly suffix of a constraint, or by using the AIMMS routine GMP::Row::SetRelaxationOnly.





Adding nonlinear constraints to a model and identifying them to be used for relaxation-only purposes can considerably speed up the solution process.





**Learn more about** 

*	:ref:`sec:var.constr`  
*	:any:`GMP::Row::SetRelaxationOnly`




**References** 

*	Sahinidis, N. V. and M. Tawarmalani, Accelerating branch-and-bound through a modeling language construct for relaxation-specific constraints, Journal of Global Optimization **32**  (2005), pp. 259-280.
*	Sherali, H. D. and W. P. Adams, A Reformulation-Linearization Technique for Solving Discrete and Continuous Nonconvex Problems, Vol. 31 of Nonconvex Optimization and its Applications, Kluwer Academic Publishers, Dordrecht, 1999.
*	Sherali, H. D., W. P. Adams and P. J. Driscoll, Exploiting special structures in constructing a hierarchy of relaxations for 0-1 mixed integer programs, Operations Research **46**  (1999), pp. 396–405.



