.. _option-ODHCPLEX-qp_linearization:


QP Linearization
================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Automatic



This option controls the linearization of the quadratic terms in the objective function of a QP or MIQP model. Possible values are:



    *	Automatic
    *	Off
    *	On




In a convex mixed integer quadratic program (MIQP), this option controls whether CPLEX linearizes the product of binary variables in the objective function during presolve.





In a nonconvex quadratic program (QP) or mixed integer quadratic program (MIQP) solved to global optimality according to the option **Solution Target**, this option controls how CPLEX linearizes the product of bounded variables in the objective function during presolve.





This option interacts with the option **Solution Target** :





*   When the solution target is set to 'Search for convex optimum' (that is, CPLEX searches for a globally optimal solution to a convex model), then in a convex MIQP, this option tells CPLEX to replace the product of a binary variable and a bounded linear variable by a linearly constrained variable.
*   When the solution target is set to 'Search for global optimum', then in a nonconvex QP or nonconvex MIQP, this option controls the initial relaxation.




**Learn more about** 

*	:ref:`option-ODHCPLEX-solution_target`  
