

.. _option-AIMMS-presolve_dual_reductions:


Presolve Dual Reductions
========================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	On	


This option controls whether the AIMMS Presolver should apply dual reductions. Possible values are:

    *	Off
    *	On


Dual reduction techniques remove feasible or even optimal solutions while guaranteeing that at least
one optimal solution remains, as long as the original problem was feasible.

For example, assume that the binary variable :math:`y` does not appear in the objective. Furthermore,
we assume that :math:`y` only appears in one constraint in the math program, namely in:

.. math::

    x + y + z <= 1

In any feasible solution in which :math:`y` equals 1 we can change its solution value to 0 while the solution remains
feasible without changing the objective value. Therefore we can fix :math:`y` to 0.


**Note** 

*	Dual reductions are automatically switched off if the model uses lazy constraints (either through a callback or a pool).
*	This option has only an effect when solving a nonlinear model and the option **Nonlinear Presolve** is switched on, or when solving a linear, quadratic or quadratically-constrained model and the option **Linear Presolve** is switched on, or if the function :any:`GMP::Instance::CreatePresolved` is used.


**Learn more about** 

*	:ref:`option-AIMMS-linear_presolve` 
*	:ref:`option-AIMMS-nonlinear_presolve`  



