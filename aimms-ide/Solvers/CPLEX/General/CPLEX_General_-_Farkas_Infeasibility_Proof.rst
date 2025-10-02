.. _option-CPLEX-farkas_infeasibility_proof:


Farkas Infeasibility Proof
==========================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	No	



This option specifies whether CPLEX should retrieve a Farkas infeasibility proof once CPLEX detects that the model is infeasible.
Possible values of this option are:

    *	No
    *	Yes


Assume the values returned for the constraints are stored in an array :math:`y[]` which has the following interpretation.
For the *i*\ -th constraint, if that constraint is a less-than-or-equal-to constraint, :math:`y[i] \leq 0` holds; if that
constraint is a greater-than-or-equal-to constraint, :math:`y[i] \geq 0` holds. Thus, where :math:`b` is the right-hand-side
vector for the given linear program, :math:`A` is the constraint matrix, and :math:`x` denotes the vector of variables,
:math:`y` may be used to derive the following valid inequality:

.. math::

   y^TA x \geq y^Tb


Here :math:`y` is being interpreted as a column vector, and math:`y^T` denotes the transpose of :math:`y`. The real point of
computing :math:`y` is the following. Suppose we define a vector :math:`z` of dimension equal to the dimension of :math:`x`
and having the following value for entries

.. math::

   z_j & = u_j \quad & \text{where} \enspace & y^TA_j > 0, \text{ and} \\
   z_j & = l_j \quad & \text{where} \enspace & y^TA_j < 0,


where :math:`A_j` denotes the column of :math:`A` corresponding to :math:`x_j`, :math:`u_j` the given upper bound on :math:`x_j`,
and :math:`l_j` is the specified lower bound. (:math:`z_j` is arbitrary if :math:`y^TA_j = 0`.) Then :math:`y` and :math:`z`
will satisfy

.. math::

   y^Tb - y^TA z > 0.


This last inequality contradicts the validity of :math:`y^TA x >= y^Tb`, and hence shows that the given linear program is infeasible.

The constraint values in the Farkas infeasibility proof are passed to AIMMS instead of the normal level values for the constraints.
Note that the general solvers option **Always Store Constraint Levels** should be switched on.

The quantity :math:`y^Tb - y^TA z` in some sense denotes the degree of infeasibility. It is stored in the .SumOfInfeasibilities suffix
of the math program.


**Note** 

*	The Farkas infeasibility proof is only available for LP and RMIP models.
*	If the presolver detects infeasibility (or indicates that the model is 'InfeasibleOrUnbounded') then the Farkas infeasibility proof is not available. In that case, turn **Presolve** off and reoptimize to obtain the Farkas infeasibility proof.
*	If you are using the barrier optimizer without crossover (see the option **LP Method**) then the Farkas infeasibility proof is not available. 


**Learn more about** 

*	:ref:`option-AIMMS-always_store_constraint_levels`  
*	:ref:`option-CPLEX-lp_method`  
*	:ref:`option-CPLEX-presolve`  
