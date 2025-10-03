.. _option-CPLEX-bqp_cuts:


BQP Cuts
========



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Automatic	



This option controls the addition of cuts based on the Boolean Quadric Polytope (BQP) for nonconvex quadratic programs (QP)
or nonconvex mixed integer quadratic programs (MIQP) solved to global optimality, that is, if the option **Solution Target**
is set to 'Search for global optimum'. Setting the value to 'Automatic', the default, indicates that the attempt to BQP cuts
should continue only if it seems to be helping. Possible values are:

    *	Off
    *	Automatic
    *	Generate cuts moderately
    *	Generate cuts aggressively
    *	Generate cuts very aggressively


BQP cuts exploit a cutting plane technique to solve QP or MIQP problems more efficiently. This technique is based on the
observation that every valid linear cut for the mixed integer set defined by:

.. math::

    A = { (x, X) : x \text{in } {0,1}, X_{ij} = x_i x_j \text{ if } i \text{ is different from } j, X_{ii} = 0 }


is also a valid inequality for the continuous set defined by:

.. math::

    B = { (x, X) : 0 \leq x \leq 1, X_{ij} = x_i x_j \text{ if } i \text{ is different from } j, X_{ii} = 0 }


**Note** 

*	CPLEX does not apply BQP cuts to mixed integer linear programs (MIP).


**Learn more about** 

*	:ref:`option-CPLEX-solution_target`  
